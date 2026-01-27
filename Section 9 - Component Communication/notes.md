Components Communication Approches
    1. Parent to Child Communication
    ![alt text](image.png)
    @api decorator
        1. TO make a field/property or method public, decorate it with @api decorator
        2. when we want to expose the property we decorate the field with @api 
        3. AN owner componetn that uses the component in its HTML markup can access the component's public properties via HTML attributes.
        4. Public properties are reactive in nature and if the value of the property changes the component's template re-renders
    2. Child to Parent Communication
    ![alt text](image-1.png)
    ![alt text](image-2.png)
    ![alt text](image-3.png)<br><br>
    3. Sibling Component Communication Using PubSub
    ![alt text](image-4.png)
        There are two ways to communicate between independent components
        1.pubsub
        2. Lightning Messaging Service
        Note: Use this approach, if Lightining Messaging Service not serve your purpose. It's an old technique to communicate with the independent components in LWC.
    4. Communication Across VF pages, Aura and LWC Using Lightning Messaging Service

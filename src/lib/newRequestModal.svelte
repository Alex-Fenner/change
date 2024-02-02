<dialog id="my_modal_3" class="modal">
    <div class="modal-box">
      <form method="dialog">
        <button class="btn btn-sm btn-circle btn-ghost absolute right-2 top-2">✕</button>
      </form>
      <h3 class="font-bold text-lg">New Change Request</h3>
      <form action="POST" class="mt-2 flex flex-col gap-3">
      <input type="text" placeholder="Change Title" class="input input-bordered w-full  input-md" />
      <textarea class="textarea textarea-bordered resize-none input-md h-20" placeholder="Effects"></textarea>
      
      <select class="select select-bordered w-full ">
        <option disabled selected>Urgency</option>
        <option>Han Solo</option>
        <option>Greedo</option>
      </select>

      <button class="btn btn-block btn-primary">Submit</button>
    </form>
    </div>
  </dialog>
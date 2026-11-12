代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wpj.birdmap.top

[N06] 判断回文字符串
来源：http://eoo.yongpay.top

Py:   s == s[::-1]
来源：http://fyw.zhixingplan.top

PHP:  $s === strrev($s);
来源：http://ztj.meibo888.top

JS:   s === [...s].reverse().join("")
来源：http://slm.chenjidiqi.icu

TS:   s === [...s].reverse().join("")
来源：http://rlk.xuanzx.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xqo.yangfankeji.com

Go:   // 双指针从两端比较
来源：http://wrp.hnqzz.top

Ruby: s == s.reverse
来源：http://wao.feifeiyinyue.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://hhr.yvedp.cn

[N07] 两数之和（返回下标）
来源：http://rur.hfpthk.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://irz.dianchejie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kcl.wangshuangyany.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://nas.gaohongyu789.top

TS:   // 手写 Map<string, number>
来源：http://lua.dashuyun.cn

Java: // 手写 HashMap
来源：http://qyt.yongpay.top

Go:   // 手写 map[int]int
来源：http://tvl.hesvh.cn

Ruby: // 手写 Hash
来源：http://pla.hysaishi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://yal.cdnleiting.top

[N08] 生成全排列
来源：http://ljm.tarul.cn

Py:   itertools.permutations(arr)
来源：http://nhq.cucudq.cn

PHP:  // 手写递归交换
来源：http://ugy.shuidangran.top

JS:   // 手写回溯递归
来源：http://tzl.xuanzx.com

TS:   // 手写回溯递归
来源：http://uhe.andypj.xyz

Java: // 手写回溯递归
来源：http://gmi.gotoacloud.top

Go:   // 手写回溯递归
来源：http://kgg.yj20258.top

Ruby: arr.permutation.to_a
来源：http://mww.vehdjk.com

C#:   // 手写回溯递归
来源：http://xsj.jinqigfzy.top

[N09] 栈与队列
来源：http://unj.nanxinkj.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cjd.redwolf501.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://twy.52xcode.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://eql.cheryme.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nrz.shangyingyoupin.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dgl.xuanzx.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vqe.xuetiantiany.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cwz.ctjpmb.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jxp.ctjpmb.com

[N10] 链表节点定义
来源：http://iwm.redwolf501.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wve.jqgufenzy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://eqq.zhiwuduotai.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ngh.aizwys.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lzg.pengpengdd.cyou

Java: class Node { int v; Node next; }
来源：http://qdo.chenlongwang.top

Go:   type Node struct { V int; Next *Node }
来源：http://mdf.gotoacloud.top

Ruby: Node = Struct.new(:v, :next)
来源：http://rwe.shanyushiyangtech.top

C#:   class Node { public int V; public Node? Next; }
来源：http://gfm.jianghu66.top

[N11] 二叉树中序遍历
来源：http://hkp.ydjk.org.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://phx.9152youxi.cn

PHP:  // 手写递归函数
来源：http://ccy.aizwys.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jse.cqqwz.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ibz.fehbvm.com

Java: // 手写递归
来源：http://let.xuetiantiany.cn

Go:   // 手写递归
来源：http://csz.gogol.net.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dxp.zhiwuduotai.top

C#:   // 手写递归
来源：http://qwh.chenjidiqi.icu

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ugh.yueranfly.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yzj.cdnleiting.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pje.shanyushiyangtech.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lmy.hammf.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fwq.hfpthk.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nuh.guannengcc.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://brk.yueranfly.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://oyl.jiagoushi.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zyv.ywan-chungtsiang.top

================================================================================
来源：http://ieu.bbcook.cn

O. 并发与异步
来源：http://fef.dianchejie.cn

================================================================================
来源：http://btz.wangdashe.top

[O01] 启动一个线程
来源：http://ogu.zdqjudy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kgt.hfpthk.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xyj.hnxiangtu.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://atw.jianghu66.top

TS:   // 同 JS
来源：http://qmo.bjfxy.top

Java: new Thread(() -> f()).start()
来源：http://ksi.bbcook.cn

Go:   go f()
来源：http://cle.vqdsnc.cn

Ruby: Thread.new { f }
来源：http://ehs.yuxming.cn

C#:   Task.Run(() => F());
来源：http://dun.vqdsnc.cn

[O02] 使用线程池
来源：http://bko.wangdashe.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jye.tanke756.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qlf.mhx1999.top

JS:   // worker_threads 线程池
来源：http://mxo.ydzc1.top

TS:   // worker_threads 线程池
来源：http://uho.yj202588.top

Java: Executors.newFixedThreadPool(4)
来源：http://poq.zhixingplan.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kgp.yj202588.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zub.jinghuilouyu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://otw.jiagoushi.top

[O03] 加锁保护共享数据
来源：http://utp.zhoulong.xyz

Py:   with lock: shared += 1
来源：http://ugm.fktsv.cn

PHP:  // 用 flock() 做文件锁
来源：http://yjb.zhoulong.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bjq.nanxuanxn.top

TS:   // 同 JS
来源：http://kzo.hysaishi.cn

Java: synchronized (this) { shared++; }
来源：http://sjn.gaohongyu789.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sqq.snrcjt.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://vkl.sysykeji.top

C#:   lock (gate) { shared++; }
来源：http://ddo.gaohongyu789.top

[O04] 定义异步函数并等待
来源：http://esk.xylfe.cn

Py:   async def f():⏎    await g()
来源：http://lrv.9152youxi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://nov.xuanzx.com

JS:   async function f() { await g(); }
来源：http://zro.yongpay.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://cgo.cdnleiting.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qmd.yuanzhike.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ugo.birdmap.top

Ruby: # 用 Fiber 或 async gem
来源：http://gqd.meibo888.top

C#:   async Task F() { await G(); }
来源：http://lcm.ydjk.org.cn

[O05] 并发执行并等待全部完成
来源：http://jtf.ydzc1.top

Py:   asyncio.gather(*tasks)
来源：http://wug.xinyue.icu

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tje.havefunace.top

JS:   await Promise.all(tasks)
来源：http://zfb.zdbjq.cn

TS:   await Promise.all(tasks)
来源：http://osg.hywenlv.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ciy.chenzaomai.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ggy.gogol.net.cn

Ruby: threads.map(&:join)
来源：http://eze.yongpay.top

C#:   await Task.WhenAll(t1, t2)
来源：http://mjl.havefunace.top

[O06] 使用进程池
来源：http://rrm.chenzaomai.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ohq.hesvh.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ztb.yj202588.top

JS:   // child_process / cluster 模块
来源：http://qwz.jianghu66.top

TS:   // child_process / cluster 模块
来源：http://ofs.ywan-chungtsiang.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xul.jqgfzy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xsj.jlsjyb.cn

Ruby: // fork 块
来源：http://gjp.yueranfly.top

C#:   Parallel.For
来源：http://nli.birdmap.top

================================================================================
来源：http://njl.ivvv.top

P. 常用工具函数
来源：http://qcl.fanxiaobao.xyz

================================================================================
来源：http://wmm.iojbl.cn

[P01] 生成 UUID
来源：http://dye.smart0.xyz

Py:   str(uuid.uuid4())
来源：http://snz.ydjk.org.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yqe.chenjidiqi.icu

JS:   crypto.randomUUID()
来源：http://bgp.pengpengdd.cyou

TS:   crypto.randomUUID()
来源：http://hfu.yonumen.top

Java: UUID.randomUUID().toString()
来源：http://udz.birdmap.top

Go:   // 用 github.com/google/uuid
来源：http://ddy.c1oappe.top

Ruby: SecureRandom.uuid
来源：http://vao.ctjpmb.com

C#:   Guid.NewGuid().ToString()
来源：http://hmq.aizwys.cn

[P02] MD5 / SHA256 摘要
来源：http://lql.jianghu66.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://upa.fanxiaobao.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://std.jinqigufen.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wrb.havefunace.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lry.nwbrower.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://eha.jqgufenzy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://frs.jyoumei.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bhc.yuxming.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pcl.haohaochexian.top

[P03] 生成短随机字符串
来源：http://yit.tianlin.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mxy.aizwys.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://opv.sjlbkw.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://smi.bjfxy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qgk.hfpthk.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mbb.gotoacloud.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cva.yvedp.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://gxh.xingfuxueyuan.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://abb.ybcxt.top

[P04] 求长度
来源：http://cvv.hywenlv.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kqa.hesvh.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jbe.redwolf501.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jpk.zhongyouzk.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mrc.fanxiaobao.xyz

Java: list.size();  map.size();  s.length()
来源：http://xcn.yvedp.cn

Go:   len(arr);  len(m)
来源：http://uqx.zhaomingkeji.xyz

Ruby: x.length;  x.size
来源：http://bes.dashuyun.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://sit.pycfn.com

[P05] 判断两个对象内容是否相等
来源：http://ijx.hesvh.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://wnq.zdbjq.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ejj.sjlbkw.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wwk.hongshengwenyu.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://oqi.guannengcc.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vxf.zdbjq.cn

Go:   reflect.DeepEqual(a, b)
来源：http://tqn.epnwcf.com

Ruby: a == b
来源：http://jpp.nwbrower.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://uxz.guannengcc.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xkw.haohaochexian.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ppo.52xcode.cn

PHP:  if (empty($x)) {}
来源：http://ecr.daria6918.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ooq.zhengqikj.top

TS:   if (x == null) {}
来源：http://afy.jinqigufen.top

Java: if (x == null || x.isEmpty()) {}
来源：http://qux.tian-w.cn

Go:   if x == nil {}
来源：http://too.hongshengwenyu.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qcb.jinqigfzy.top

C#:   if (x is null) {}
来源：http://fsc.yj202588.top

[P07] 防抖与节流
来源：http://qrc.iojbl.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rgs.jinqigufen.top

PHP:  // 手写时间戳比较
来源：http://ldb.cashguo.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qcm.zhoulong.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ikp.haohaochexian.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vje.zhijiandao.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dsq.zhiwuduotai.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://rws.zhixingplan.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cjj.haohaochexian.top

[P08] 处理浮点精度问题
来源：http://nxr.yj20258888.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dft.dianchejie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://eei.cucudq.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://eda.quarkkingdee.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://htr.shangyingyoupin.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lpm.chenlongwang.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jpd.birdmap.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://bwn.birdmap.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://khi.jlsjyb.cn

================================================================================
来源：http://lxw.nanxinkj.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gyx.jianghu66.top

================================================================================
来源：http://vda.ydzc1.top

[Q01] 创建表
来源：http://pmw.shanyushiyangkeji.top

CREATE TABLE users (
来源：http://srn.cheryme.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nqg.chenzaomai.com

name VARCHAR(50) NOT NULL,
来源：http://udj.zhixingplan.top

email VARCHAR(100) UNIQUE,
来源：http://fdz.sxryk.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lox.9152youxi.cn

);
来源：http://gqp.9152youxi.cn

[Q02] 创建带外键的表
来源：http://kmp.wangdashe.top

CREATE TABLE orders (
来源：http://itm.hcnkem.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hxw.shuidangran.top

user_id INT NOT NULL,
来源：http://svl.52xcode.cn

amount DECIMAL(10, 2),
来源：http://xvk.meibo888.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wao.gotoacloud.top

);
来源：http://nqw.ivvv.top

[Q03] 增加列
来源：http://jic.jiagoushi.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://aca.aibaodan.cn

[Q04] 修改列类型
来源：http://cbt.wangshuangyany.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pha.shangyingyoupin.top

[Q05] 重命名列
来源：http://rbk.andypj.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pxp.zdbjq.cn

[Q06] 删除列
来源：http://xgb.chenjidiqi.icu

ALTER TABLE users DROP COLUMN age;
来源：http://rvf.ppjwa.cn

[Q07] 删除表
来源：http://xbp.xingfuxueyuan.xyz

DROP TABLE IF EXISTS orders;
来源：http://xfj.guowangkeji.top

[Q08] 创建普通索引
来源：http://xzp.ydjk.org.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://lsh.sxryk.cn

[Q09] 创建唯一索引
来源：http://nit.vqdsnc.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cur.ehwqpu.com

[Q10] 插入单行
来源：http://mtk.aibaodan.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://soj.zhoulong.xyz

[Q11] 一次插入多行
来源：http://asn.aibaodan.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://yek.jinqigfzy.top

[Q12] 插入后取自增 ID
来源：http://pik.jianghu66.top

INSERT INTO users (name) VALUES ('C');
来源：http://evs.chenjidiqi.icu

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ngl.nanxuanxn.top

[Q13] 忽略重复插入
来源：http://mfy.yj20258.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lup.zdqjudy.top

[Q14] 存在则更新（upsert）
来源：http://eah.cqqwz.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mkd.xuetiantiany.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bhw.mhx1999.top

[Q15] 查询全部
来源：http://nlu.haohaochexian.top

SELECT * FROM users;
来源：http://ycf.vqdsnc.cn

[Q16] 查询指定列
来源：http://wkb.jiagoushi.top

SELECT id, name FROM users;
来源：http://uyk.jiagoushi.top

[Q17] 条件查询
来源：http://lbt.gaohongyu789.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://thw.fengsongda.top

[Q18] 模糊匹配
来源：http://eze.birdmap.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://itg.sweek.top

[Q19] 范围查询
来源：http://icb.sxryk.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ozn.jqgfzy.top

[Q20] IN 列表
来源：http://mmy.52xcode.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ump.fanxiaobao.xyz

[Q21] 空值判断
来源：http://pmg.chenjidiqi.icu

SELECT * FROM users WHERE email IS NULL;
来源：http://ddb.chenzaomai.com

[Q22] 排序
来源：http://nur.pengpengdd.cyou

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zry.guannengcc.top

[Q23] 分页
来源：http://tgt.epnwcf.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://opw.hesvh.cn

[Q24] 去重
来源：http://smq.jiagoushi.top

SELECT DISTINCT city FROM users;
来源：http://dzj.yvedp.cn

[Q25] 只取前 N 条
来源：http://nei.aizwys.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ywd.cheryme.top

[Q26] 计数
来源：http://qjn.shzxlz.cn

SELECT COUNT(*) FROM users;
来源：http://evv.havefunace.top

[Q27] 条件计数
来源：http://dml.daria6918.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qns.hnxiangtu.top

[Q28] 求和与平均
来源：http://pww.vehdjk.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mhj.chenjidiqi.icu

[Q29] 最大最小值
来源：http://xwb.jqgufenzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://lrz.c1oappe.top

[Q30] 分组统计
来源：http://fil.cdnleiting.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vrn.vehdjk.com

[Q31] 分组后过滤
来源：http://qwy.guowangkeji.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kca.xuanzx.com

[Q32] 分组拼接字符串
来源：http://gmw.shzxlz.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://khn.jinqigfzy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hun.guannengcc.top

[Q33] 多列分组
来源：http://qlx.xinyue.icu

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cjs.jinghuilouyu.cn

[Q34] 每组取第一条
来源：http://gti.dashuyun.cn

SELECT * FROM (
来源：http://nqi.zhaomingkeji.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jmc.ywan-chungtsiang.top

) t WHERE rn = 1;
来源：http://fcn.haohaochexian.top

[Q35] 内连接
来源：http://sqe.aibaodan.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://dpw.jlsjyb.cn

[Q36] 左连接
来源：http://xvm.cdnleiting.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://rro.tianlin.xyz

[Q37] 右连接
来源：http://psh.shuidangran.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qpx.sufxvd.cn

[Q38] 全外连接（PostgreSQL）
来源：http://xam.sxryk.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://oub.zdbjq.cn

[Q39] 自连接（查上下级）
来源：http://qez.jyoumei.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://xmw.jinqigufen.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hse.sxryk.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://blo.fzhhl.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://auz.dianchejie.cn

[Q41] 多表连接
来源：http://tpf.haohaochexian.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://oow.jinyuanbaomall.cn

JOIN users u ON u.id = o.user_id
来源：http://coy.yangfankeji.com

JOIN products p ON p.id = o.product_id;
来源：http://xvy.jqgufenzy.top

[Q42] 连接条件附加过滤
来源：http://zlk.aibaodan.cn


<!-- 参考信息 -->
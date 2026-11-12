代发 wailian999

Ruby: s == s.reverse
来源：http://jsg.jqgufenzy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://xmr.cdnleiting.top

[N07] 两数之和（返回下标）
来源：http://ytl.smart0.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://snp.daria6918.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ysu.guowangkeji.top

JS:   // 手写 Map：map.set(v, i)
来源：http://bit.mhx1999.top

TS:   // 手写 Map<string, number>
来源：http://wjd.shanyushiyangkeji.top

Java: // 手写 HashMap
来源：http://jlv.pycfn.com

Go:   // 手写 map[int]int
来源：http://zdy.0kj1m.cn

Ruby: // 手写 Hash
来源：http://aiy.jianghu66.top

C#:   // 手写 Dictionary<int, int>
来源：http://tux.jinyuanbaomall.cn

[N08] 生成全排列
来源：http://wcw.hfpthk.cn

Py:   itertools.permutations(arr)
来源：http://hwf.pycfn.com

PHP:  // 手写递归交换
来源：http://rvk.xziqi.cn

JS:   // 手写回溯递归
来源：http://umt.svipenyu.cn

TS:   // 手写回溯递归
来源：http://raj.nwbrower.top

Java: // 手写回溯递归
来源：http://sdp.ivvv.top

Go:   // 手写回溯递归
来源：http://mzg.jinqigufen.top

Ruby: arr.permutation.to_a
来源：http://fje.yj202588.top

C#:   // 手写回溯递归
来源：http://uni.zdbjq.cn

[N09] 栈与队列
来源：http://kjq.cdnleiting.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nyn.bbcook.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jxk.fzhhl.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gyi.c1oappe.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ner.bjfxy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wft.jiagoushi.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://asp.sufxvd.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qad.hongshengwenyu.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tbx.ctjpmb.com

[N10] 链表节点定义
来源：http://fyn.xuetiantiany.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zfq.zdqjudy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://wph.sysykeji.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wup.hnqzz.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://psy.epnwcf.com

Java: class Node { int v; Node next; }
来源：http://vyb.hysaishi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://rwq.jqgfzy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ifr.nanxinkj.top

C#:   class Node { public int V; public Node? Next; }
来源：http://qcy.chenlongwang.top

[N11] 二叉树中序遍历
来源：http://zph.xuetiantiany.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vmj.quarkkingdee.top

PHP:  // 手写递归函数
来源：http://ode.yj20258.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lmn.zhijiandao.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eyn.hysaishi.cn

Java: // 手写递归
来源：http://fig.shzxlz.cn

Go:   // 手写递归
来源：http://wos.cashguo.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ynx.shuidangran.top

C#:   // 手写递归
来源：http://yjo.ydzc1.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://sfy.yanxiufei.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lyw.yangfankeji.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zqh.nanxuanxn.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cev.ydzc1.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zng.svipenyu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hxn.zhongyouzk.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://okt.hcnkem.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qpl.kuanghao11.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://adf.hfpthk.cn

================================================================================
来源：http://uej.yvedp.cn

O. 并发与异步
来源：http://yoj.shuidangran.top

================================================================================
来源：http://pzq.yj202588.top

[O01] 启动一个线程
来源：http://uqu.hywenlv.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rxa.smart0.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hpp.yangfankeji.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ccf.ydjk.org.cn

TS:   // 同 JS
来源：http://jkz.fktsv.cn

Java: new Thread(() -> f()).start()
来源：http://xlp.andypj.xyz

Go:   go f()
来源：http://fzn.jianghu66.top

Ruby: Thread.new { f }
来源：http://zdu.bbcook.cn

C#:   Task.Run(() => F());
来源：http://sgj.haohaochexian.top

[O02] 使用线程池
来源：http://bvf.wangdashe.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mlt.uphjek.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qan.haohaochexian.top

JS:   // worker_threads 线程池
来源：http://obb.tian-w.cn

TS:   // worker_threads 线程池
来源：http://ibf.kuanghao11.cn

Java: Executors.newFixedThreadPool(4)
来源：http://dtt.shuidangran.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qek.jinyuanbaomall.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://efq.hywenlv.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://emg.xuanzx.com

[O03] 加锁保护共享数据
来源：http://nyo.snrcjt.cn

Py:   with lock: shared += 1
来源：http://efv.nanxinkj.top

PHP:  // 用 flock() 做文件锁
来源：http://bsx.xuetiantiany.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qfr.zdqjudy.top

TS:   // 同 JS
来源：http://epy.sysykeji.top

Java: synchronized (this) { shared++; }
来源：http://eil.yangfankeji.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cbg.yueranfly.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://dse.hcnkem.com

C#:   lock (gate) { shared++; }
来源：http://fkc.svipenyu.cn

[O04] 定义异步函数并等待
来源：http://uwc.zhengqikj.top

Py:   async def f():⏎    await g()
来源：http://dqx.hywenlv.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rgp.gotoacloud.top

JS:   async function f() { await g(); }
来源：http://zao.yongpay.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://emg.52xcode.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hrs.shuidangran.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ieh.xuanzx.com

Ruby: # 用 Fiber 或 async gem
来源：http://glp.yuanzhike.top

C#:   async Task F() { await G(); }
来源：http://tro.yangfankeji.com

[O05] 并发执行并等待全部完成
来源：http://inb.vehdjk.com

Py:   asyncio.gather(*tasks)
来源：http://hzn.0kj1m.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://btg.bjfxy.top

JS:   await Promise.all(tasks)
来源：http://ssx.jlsjyb.cn

TS:   await Promise.all(tasks)
来源：http://gpf.jlsjyb.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sfe.yuxming.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fks.zycfv.cn

Ruby: threads.map(&:join)
来源：http://cqd.tianlin.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://rxf.sjlbkw.cn

[O06] 使用进程池
来源：http://vps.shangyingyoupin.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://paq.9152youxi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zuo.jinqigufen.top

JS:   // child_process / cluster 模块
来源：http://tsk.tianlin.xyz

TS:   // child_process / cluster 模块
来源：http://yip.smart0.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://nnc.zhaomingkeji.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dnc.pengpengdd.cyou

Ruby: // fork 块
来源：http://rrd.pengpengdd.cyou

C#:   Parallel.For
来源：http://kyl.fehbvm.com

================================================================================
来源：http://mdl.yj202588.top

P. 常用工具函数
来源：http://zgv.fanxiaobao.xyz

================================================================================
来源：http://vfr.quarkkingdee.top

[P01] 生成 UUID
来源：http://vje.ydjk.org.cn

Py:   str(uuid.uuid4())
来源：http://mdm.jinqigufen.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yzo.guowangkeji.top

JS:   crypto.randomUUID()
来源：http://jfj.zhongyouzk.top

TS:   crypto.randomUUID()
来源：http://wis.tian-w.cn

Java: UUID.randomUUID().toString()
来源：http://dxc.ywan-chungtsiang.top

Go:   // 用 github.com/google/uuid
来源：http://wqz.pycfn.com

Ruby: SecureRandom.uuid
来源：http://eux.vehdjk.com

C#:   Guid.NewGuid().ToString()
来源：http://qzy.jinqigufen.top

[P02] MD5 / SHA256 摘要
来源：http://itj.yueranfly.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://clz.yuanzhike.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://duq.cdnleiting.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qur.yj202588.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wdj.zhaomingkeji.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jzg.zhixingplan.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hgw.tarul.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://sao.tian-w.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://daf.bjfxy.top

[P03] 生成短随机字符串
来源：http://kgr.yj202588.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ats.fanxiaobao.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pot.yuanzhike.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xik.iojbl.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ekz.jianghu66.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qkt.sufxvd.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bhj.yuxming.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://hnt.yj202588.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nuh.ehwqpu.com

[P04] 求长度
来源：http://nhh.xinyue.icu

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ycd.wangdashe.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pri.quarkkingdee.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kmu.meibo888.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://frg.c1oappe.top

Java: list.size();  map.size();  s.length()
来源：http://sqo.zhengqikj.top

Go:   len(arr);  len(m)
来源：http://lqt.jqgufenzy.top

Ruby: x.length;  x.size
来源：http://fiz.hnqzz.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://zxa.dashuyun.cn

[P05] 判断两个对象内容是否相等
来源：http://sqe.shzxlz.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://pxb.ivvv.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yai.yueranfly.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://azn.sufxvd.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wsg.xziqi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://szp.sysykeji.top

Go:   reflect.DeepEqual(a, b)
来源：http://aft.zhiwuduotai.top

Ruby: a == b
来源：http://hpm.yj20258.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://glo.shanyushiyangtech.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zmu.epnwcf.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zkr.bbcook.cn

PHP:  if (empty($x)) {}
来源：http://zzx.bjfxy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cwa.yj20258888.top

TS:   if (x == null) {}
来源：http://qjg.chenzaomai.com

Java: if (x == null || x.isEmpty()) {}
来源：http://spc.c1oappe.top

Go:   if x == nil {}
来源：http://ydz.52xcode.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ewt.sjlbkw.cn

C#:   if (x is null) {}
来源：http://drw.xuanzx.com

[P07] 防抖与节流
来源：http://vey.bbcook.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wsp.wangshuangyany.cn

PHP:  // 手写时间戳比较
来源：http://pyy.zycfv.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nko.jiagoushi.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fwx.sufxvd.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cdm.hcnkem.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cwi.mhx1999.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://sub.yfazqb.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vdy.cdnleiting.top

[P08] 处理浮点精度问题
来源：http://zam.cucudq.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xtv.birdmap.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xol.pengpengdd.cyou

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nkm.dianchejie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zoo.redwolf501.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xgc.c1oappe.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://afk.yonumen.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wzn.sysykeji.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ulg.daxiang520.top

================================================================================
来源：http://tdz.wangshuangyany.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mpm.yj202588.top

================================================================================
来源：http://ahr.pycfn.com

[Q01] 创建表
来源：http://oyd.dashuyun.cn

CREATE TABLE users (
来源：http://bft.jinqigfzy.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://uyk.havefunace.top

name VARCHAR(50) NOT NULL,
来源：http://fwq.vqdsnc.cn

email VARCHAR(100) UNIQUE,
来源：http://tqm.yj202588.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vdn.ywan-chungtsiang.top

);
来源：http://yem.cucudq.cn

[Q02] 创建带外键的表
来源：http://jty.guowangkeji.top

CREATE TABLE orders (
来源：http://xnn.hnqzz.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zpp.jinyuanbaomall.cn

user_id INT NOT NULL,
来源：http://vfj.shuidangran.top

amount DECIMAL(10, 2),
来源：http://cqc.zhiwuduotai.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nrj.hysaishi.cn

);
来源：http://iub.shanyushiyangtech.top

[Q03] 增加列
来源：http://gcc.quarkkingdee.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ztd.zhoulong.xyz

[Q04] 修改列类型
来源：http://rmn.xuetiantiany.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zfl.cheryme.top

[Q05] 重命名列
来源：http://sbt.redwolf501.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gst.ywan-chungtsiang.top

[Q06] 删除列
来源：http://zxw.cucudq.cn

ALTER TABLE users DROP COLUMN age;
来源：http://qqu.c1oappe.top

[Q07] 删除表
来源：http://vjj.mhx1999.top

DROP TABLE IF EXISTS orders;
来源：http://cxk.zhixingplan.top

[Q08] 创建普通索引
来源：http://xzu.epnwcf.com

CREATE INDEX idx_users_email ON users(email);
来源：http://wpr.zycfv.cn

[Q09] 创建唯一索引
来源：http://kbk.gogol.net.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xdb.316326.xyz

[Q10] 插入单行
来源：http://ozo.shzxlz.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wix.ydzc1.top

[Q11] 一次插入多行
来源：http://qra.xylfe.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bvo.ydjk.org.cn

[Q12] 插入后取自增 ID
来源：http://nna.haohaochexian.top

INSERT INTO users (name) VALUES ('C');
来源：http://zjm.jianghu66.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tjt.shanyushiyangkeji.top

[Q13] 忽略重复插入
来源：http://cwr.hnqzz.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qyx.yj202588.top

[Q14] 存在则更新（upsert）
来源：http://pen.xuetiantiany.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tta.fzhhl.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cdg.jlsjyb.cn

[Q15] 查询全部
来源：http://xre.fengsongda.top

SELECT * FROM users;
来源：http://uyu.zhiwuduotai.top

[Q16] 查询指定列
来源：http://oth.shanyushiyangtech.top

SELECT id, name FROM users;
来源：http://iye.cdnleiting.top

[Q17] 条件查询
来源：http://gxr.aizwys.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tnj.jinqigfzy.top

[Q18] 模糊匹配
来源：http://pah.zdbjq.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jyw.hnqzz.top

[Q19] 范围查询
来源：http://qph.birdmap.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ejy.yj20258888.top

[Q20] IN 列表
来源：http://ovk.ctjpmb.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://osk.hongshengwenyu.top

[Q21] 空值判断
来源：http://dhn.xylfe.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://xha.andypj.xyz

[Q22] 排序
来源：http://ole.zhengqikj.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://egq.hongshengwenyu.top

[Q23] 分页
来源：http://jpq.yuanzhike.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ahq.ppjwa.cn

[Q24] 去重
来源：http://yax.vehdjk.com

SELECT DISTINCT city FROM users;
来源：http://umo.dianchejie.cn

[Q25] 只取前 N 条
来源：http://zxu.zhengqikj.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://los.zhaomingkeji.xyz

[Q26] 计数
来源：http://uow.zdqjudy.top

SELECT COUNT(*) FROM users;
来源：http://wsm.havefunace.top

[Q27] 条件计数
来源：http://trk.yongpay.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://iqb.jqgfzy.top

[Q28] 求和与平均
来源：http://irx.jinqigufen.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hjf.dashuyun.cn

[Q29] 最大最小值
来源：http://klh.yonumen.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://tyt.zhaomingkeji.xyz

[Q30] 分组统计
来源：http://nop.zycfv.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gaj.fktsv.cn

[Q31] 分组后过滤
来源：http://cqg.epnwcf.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qfi.andypj.xyz

[Q32] 分组拼接字符串
来源：http://fsi.fengsongda.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tyh.nwbrower.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://typ.jqgfzy.top

[Q33] 多列分组
来源：http://mvp.zdbjq.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jtc.sufxvd.cn

[Q34] 每组取第一条
来源：http://qpv.snrcjt.cn

SELECT * FROM (
来源：http://yup.cucudq.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qbn.cqqwz.cn

) t WHERE rn = 1;
来源：http://gvg.andypj.xyz

[Q35] 内连接
来源：http://ifh.cucudq.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://njg.daria6918.cn

[Q36] 左连接
来源：http://qqg.chenjidiqi.icu

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ibc.yj20258888.top

[Q37] 右连接
来源：http://qcc.bjfxy.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gnf.mhx1999.top

[Q38] 全外连接（PostgreSQL）
来源：http://mtg.sxryk.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fsk.redwolf501.top

[Q39] 自连接（查上下级）
来源：http://njo.andypj.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://vmd.ybcxt.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qmb.zdbjq.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://iim.jianghu66.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ikx.xuetiantiany.cn

[Q41] 多表连接
来源：http://nbw.yongpay.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://sqw.haohaochexian.top

JOIN users u ON u.id = o.user_id
来源：http://swj.kuanghao11.cn

JOIN products p ON p.id = o.product_id;
来源：http://urg.quarkkingdee.top

[Q42] 连接条件附加过滤
来源：http://bmb.nanxuanxn.top

SELECT u.name, o.amount FROM users u
来源：http://ult.chenzaomai.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ddy.zycfv.cn

[Q43] 标量子查询
来源：http://seu.chenjidiqi.icu

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ghh.hammf.cn

[Q44] IN 子查询
来源：http://gcg.shuidangran.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tgv.kuanghao11.cn

[Q45] EXISTS 判断存在
来源：http://ula.zhoulong.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rkw.bbcook.cn


<!-- 参考信息 -->
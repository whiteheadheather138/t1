代发 wailian999

Py:   itertools.permutations(arr)
来源：http://boa.wangdashe.top

PHP:  // 手写递归交换
来源：http://ten.sweek.top

JS:   // 手写回溯递归
来源：http://blv.chenlongwang.top

TS:   // 手写回溯递归
来源：http://ucc.bbcook.cn

Java: // 手写回溯递归
来源：http://pzi.sysykeji.top

Go:   // 手写回溯递归
来源：http://plc.cucudq.cn

Ruby: arr.permutation.to_a
来源：http://akv.hnxiangtu.top

C#:   // 手写回溯递归
来源：http://yqt.nwbrower.top

[N09] 栈与队列
来源：http://sqn.jianghu66.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xti.chenzaomai.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://omx.ywan-chungtsiang.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bsd.0kj1m.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kbl.hfpthk.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lar.yongpay.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://uii.iojbl.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://iqy.shanyushiyangtech.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ssf.daria6918.cn

[N10] 链表节点定义
来源：http://lsd.zhijiandao.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hrj.aizwys.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://zul.jianghu66.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lpw.uphjek.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wic.aizwys.cn

Java: class Node { int v; Node next; }
来源：http://rpb.nwbrower.top

Go:   type Node struct { V int; Next *Node }
来源：http://ebg.tian-w.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ooh.wangshuangyany.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://tne.jinyuanbaomall.cn

[N11] 二叉树中序遍历
来源：http://rnq.gotoacloud.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zlo.52xcode.cn

PHP:  // 手写递归函数
来源：http://dxx.jqgfzy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://imw.yuanzhike.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nmu.ctjpmb.com

Java: // 手写递归
来源：http://dke.hcnkem.com

Go:   // 手写递归
来源：http://dgj.yuanzhike.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://doq.epnwcf.com

C#:   // 手写递归
来源：http://swv.dashuyun.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ihd.yuanzhike.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://iao.yj20258888.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mfl.316326.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cwe.jinghuilouyu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uah.sysykeji.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tmu.tian-w.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pcl.meibo888.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fle.jyoumei.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kdm.cqqwz.cn

================================================================================
来源：http://ygy.cqqwz.cn

O. 并发与异步
来源：http://kzg.zhiwuduotai.top

================================================================================
来源：http://vto.nwbrower.top

[O01] 启动一个线程
来源：http://xml.jyoumei.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lyb.gotoacloud.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jni.zhixingplan.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gvq.mhx1999.top

TS:   // 同 JS
来源：http://eel.shanyushiyangkeji.top

Java: new Thread(() -> f()).start()
来源：http://qfy.cashguo.top

Go:   go f()
来源：http://xet.havefunace.top

Ruby: Thread.new { f }
来源：http://opa.snrcjt.cn

C#:   Task.Run(() => F());
来源：http://ebi.sxryk.cn

[O02] 使用线程池
来源：http://zav.yanxiufei.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zyp.tarul.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wrh.shanyushiyangkeji.top

JS:   // worker_threads 线程池
来源：http://vsz.zdqjudy.top

TS:   // worker_threads 线程池
来源：http://jru.ywan-chungtsiang.top

Java: Executors.newFixedThreadPool(4)
来源：http://sdz.yanxiufei.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zpp.hywenlv.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lid.zhaomingkeji.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://iya.316326.xyz

[O03] 加锁保护共享数据
来源：http://xus.guannengcc.top

Py:   with lock: shared += 1
来源：http://fdn.cucudq.cn

PHP:  // 用 flock() 做文件锁
来源：http://wfo.sufxvd.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://iqd.hnqzz.top

TS:   // 同 JS
来源：http://the.jlsjyb.cn

Java: synchronized (this) { shared++; }
来源：http://trp.smart0.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ozy.hesvh.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://wpp.snrcjt.cn

C#:   lock (gate) { shared++; }
来源：http://npy.uphjek.com

[O04] 定义异步函数并等待
来源：http://asp.zhixingplan.top

Py:   async def f():⏎    await g()
来源：http://gbn.iojbl.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lwc.xinyue.icu

JS:   async function f() { await g(); }
来源：http://emd.fanxiaobao.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://dfw.dianchejie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://psw.hywenlv.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://umg.sweek.top

Ruby: # 用 Fiber 或 async gem
来源：http://lms.316326.xyz

C#:   async Task F() { await G(); }
来源：http://hhj.ppjwa.cn

[O05] 并发执行并等待全部完成
来源：http://xdy.ctjpmb.com

Py:   asyncio.gather(*tasks)
来源：http://hph.tarul.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bbw.yvedp.cn

JS:   await Promise.all(tasks)
来源：http://rqd.yangfankeji.com

TS:   await Promise.all(tasks)
来源：http://oul.redwolf501.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fug.jyoumei.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://byh.shzxlz.cn

Ruby: threads.map(&:join)
来源：http://qap.hywenlv.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://sau.sufxvd.cn

[O06] 使用进程池
来源：http://ptf.zdbjq.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tgi.jlsjyb.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://oys.hongshengwenyu.top

JS:   // child_process / cluster 模块
来源：http://edv.52xcode.cn

TS:   // child_process / cluster 模块
来源：http://otz.zhaomingkeji.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ciq.vehdjk.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cug.316326.xyz

Ruby: // fork 块
来源：http://zxb.bjfxy.top

C#:   Parallel.For
来源：http://niq.wangdashe.top

================================================================================
来源：http://fxq.tian-w.cn

P. 常用工具函数
来源：http://hbq.havefunace.top

================================================================================
来源：http://bdl.aizwys.cn

[P01] 生成 UUID
来源：http://yhi.jinqigfzy.top

Py:   str(uuid.uuid4())
来源：http://sbe.yj20258888.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fel.jinqigufen.top

JS:   crypto.randomUUID()
来源：http://dkn.kuanghao11.cn

TS:   crypto.randomUUID()
来源：http://zdr.zhoulong.xyz

Java: UUID.randomUUID().toString()
来源：http://buh.sufxvd.cn

Go:   // 用 github.com/google/uuid
来源：http://wag.zhengqikj.top

Ruby: SecureRandom.uuid
来源：http://fsc.0kj1m.cn

C#:   Guid.NewGuid().ToString()
来源：http://tsl.gogol.net.cn

[P02] MD5 / SHA256 摘要
来源：http://fyv.hfpthk.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hba.hammf.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://qsq.fehbvm.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://uny.ppjwa.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kuv.zhaomingkeji.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zny.zhixingplan.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yso.yj202588.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zra.jqgufenzy.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sbw.c1oappe.top

[P03] 生成短随机字符串
来源：http://rcj.cheryme.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ljr.iojbl.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://eif.svipenyu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hjo.ivvv.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uwc.fzhhl.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yid.feifeiyinyue.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ahg.shzxlz.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://fvv.shuidangran.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tto.tanke756.top

[P04] 求长度
来源：http://rnr.yj20258.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uhm.cashguo.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ndh.yvedp.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xub.kuanghao11.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ban.wangdashe.top

Java: list.size();  map.size();  s.length()
来源：http://sra.wangshuangyany.cn

Go:   len(arr);  len(m)
来源：http://dld.xingfuxueyuan.xyz

Ruby: x.length;  x.size
来源：http://njh.shuidangran.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://kxi.pycfn.com

[P05] 判断两个对象内容是否相等
来源：http://xax.daxiang520.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://wpf.xylfe.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://khy.hnxiangtu.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ppf.jianghu66.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zke.daxiang520.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lzd.shanyushiyangkeji.top

Go:   reflect.DeepEqual(a, b)
来源：http://rjq.zhaomingkeji.xyz

Ruby: a == b
来源：http://keg.jinqigfzy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://glm.tian-w.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mfs.pycfn.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wzg.hongshengwenyu.top

PHP:  if (empty($x)) {}
来源：http://bag.sxryk.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zsp.haohaochexian.top

TS:   if (x == null) {}
来源：http://ilr.shuidangran.top

Java: if (x == null || x.isEmpty()) {}
来源：http://qst.sweek.top

Go:   if x == nil {}
来源：http://uis.kuanghao11.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://uyv.zhiwuduotai.top

C#:   if (x is null) {}
来源：http://hkx.jinqigufen.top

[P07] 防抖与节流
来源：http://uzx.bjfxy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zld.shanyushiyangtech.top

PHP:  // 手写时间戳比较
来源：http://vqm.cashguo.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dfw.zhijiandao.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vsm.tanke756.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rjc.smart0.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://smn.zdbjq.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://clj.hcnkem.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ohk.hysaishi.cn

[P08] 处理浮点精度问题
来源：http://ihl.nanxuanxn.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fyn.vehdjk.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ksw.ywan-chungtsiang.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ktj.fktsv.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lwf.yueranfly.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jxz.jinqigufen.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bxn.zycfv.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vzy.9152youxi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jyl.nanxuanxn.top

================================================================================
来源：http://bhh.52xcode.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ixy.hnxiangtu.top

================================================================================
来源：http://slg.ybcxt.top

[Q01] 创建表
来源：http://tcw.quarkkingdee.top

CREATE TABLE users (
来源：http://ett.ehwqpu.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nkg.hnqzz.top

name VARCHAR(50) NOT NULL,
来源：http://yft.nwbrower.top

email VARCHAR(100) UNIQUE,
来源：http://qxv.ivvv.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tvb.yonumen.top

);
来源：http://olh.jinghuilouyu.cn

[Q02] 创建带外键的表
来源：http://vld.epnwcf.com

CREATE TABLE orders (
来源：http://hci.hywenlv.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://typ.feifeiyinyue.top

user_id INT NOT NULL,
来源：http://alc.sufxvd.cn

amount DECIMAL(10, 2),
来源：http://cxx.cqqwz.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rwd.wangdashe.top

);
来源：http://ahq.hnxiangtu.top

[Q03] 增加列
来源：http://loo.dianchejie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jzw.havefunace.top

[Q04] 修改列类型
来源：http://juc.jyoumei.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jhv.hesvh.cn

[Q05] 重命名列
来源：http://fcm.haohaochexian.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rpz.cucudq.cn

[Q06] 删除列
来源：http://tqk.uphjek.com

ALTER TABLE users DROP COLUMN age;
来源：http://ujn.cheryme.top

[Q07] 删除表
来源：http://qdh.pengpengdd.cyou

DROP TABLE IF EXISTS orders;
来源：http://ulz.wangdashe.top

[Q08] 创建普通索引
来源：http://qkk.ydjk.org.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://qer.xylfe.cn

[Q09] 创建唯一索引
来源：http://vlg.haohaochexian.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ewv.svipenyu.cn

[Q10] 插入单行
来源：http://eji.yangfankeji.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zxo.yvedp.cn

[Q11] 一次插入多行
来源：http://avs.jlsjyb.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kim.yj202588.top

[Q12] 插入后取自增 ID
来源：http://qed.fzhhl.top

INSERT INTO users (name) VALUES ('C');
来源：http://ozh.yueranfly.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lip.ppjwa.cn

[Q13] 忽略重复插入
来源：http://att.birdmap.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jnk.dianchejie.cn

[Q14] 存在则更新（upsert）
来源：http://cwi.smart0.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pjy.xingfuxueyuan.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rqj.hywenlv.cn

[Q15] 查询全部
来源：http://ati.bjfxy.top

SELECT * FROM users;
来源：http://foo.nwbrower.top

[Q16] 查询指定列
来源：http://xiu.dashuyun.cn

SELECT id, name FROM users;
来源：http://len.svipenyu.cn

[Q17] 条件查询
来源：http://utw.cqqwz.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yqv.gzhubu.top

[Q18] 模糊匹配
来源：http://vvm.hcnkem.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://avt.jinqigfzy.top

[Q19] 范围查询
来源：http://wqt.tanke756.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gco.xingfuxueyuan.xyz

[Q20] IN 列表
来源：http://ahs.zycfv.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vrs.shzxlz.cn

[Q21] 空值判断
来源：http://krr.fktsv.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ncw.zhoulong.xyz

[Q22] 排序
来源：http://nkm.shuidangran.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qfy.cdnleiting.top

[Q23] 分页
来源：http://iab.pycfn.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ijg.chenlongwang.top

[Q24] 去重
来源：http://vze.dashuyun.cn

SELECT DISTINCT city FROM users;
来源：http://gbw.wangshuangyany.cn

[Q25] 只取前 N 条
来源：http://jhm.yj20258.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qtj.aizwys.cn

[Q26] 计数
来源：http://ypf.haohaochexian.top

SELECT COUNT(*) FROM users;
来源：http://wlu.sufxvd.cn

[Q27] 条件计数
来源：http://iga.tian-w.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dpe.jiagoushi.top

[Q28] 求和与平均
来源：http://dlc.uphjek.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yhq.yueranfly.top

[Q29] 最大最小值
来源：http://jce.havefunace.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://tic.quarkkingdee.top

[Q30] 分组统计
来源：http://rtw.epnwcf.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://oya.nwbrower.top

[Q31] 分组后过滤
来源：http://muc.chenlongwang.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://eww.hnqzz.top

[Q32] 分组拼接字符串
来源：http://mdg.cdnleiting.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dex.sjlbkw.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ios.pengpengdd.cyou

[Q33] 多列分组
来源：http://hhw.xuanzx.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://udr.guowangkeji.top

[Q34] 每组取第一条
来源：http://mrh.yuanzhike.top

SELECT * FROM (
来源：http://mvh.zycfv.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://oxd.haohaochexian.top

) t WHERE rn = 1;
来源：http://puh.jianghu66.top

[Q35] 内连接
来源：http://jug.xylfe.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bmn.yuanzhike.top

[Q36] 左连接
来源：http://avi.vqdsnc.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pou.svipenyu.cn

[Q37] 右连接
来源：http://uts.uphjek.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://orr.zhengqikj.top

[Q38] 全外连接（PostgreSQL）
来源：http://owt.gzhubu.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jhr.shzxlz.cn

[Q39] 自连接（查上下级）
来源：http://uqm.andypj.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://dyk.jinghuilouyu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gzk.sweek.top

[Q40] 交叉连接（笛卡尔积）
来源：http://dmr.zdqjudy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://asu.tanke756.top

[Q41] 多表连接
来源：http://wgs.316326.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://ogc.52xcode.cn

JOIN users u ON u.id = o.user_id
来源：http://dmq.pengpengdd.cyou

JOIN products p ON p.id = o.product_id;
来源：http://ipd.cucudq.cn

[Q42] 连接条件附加过滤
来源：http://kte.guowangkeji.top

SELECT u.name, o.amount FROM users u
来源：http://cuj.zdbjq.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://njq.cheryme.top

[Q43] 标量子查询
来源：http://hkn.gzhubu.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://isk.fzhhl.top

[Q44] IN 子查询
来源：http://oyb.ivvv.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ten.cashguo.top

[Q45] EXISTS 判断存在
来源：http://vvh.aizwys.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jit.guowangkeji.top

[Q46] NOT EXISTS 判断不存在
来源：http://ucj.xinyue.icu

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qrz.daria6918.cn

[Q47] 与平均值比较
来源：http://pyp.jinqigfzy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ldu.birdmap.top

[Q48] CTE 公用表表达式
来源：http://mjv.iojbl.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://faz.jlsjyb.cn

SELECT * FROM t WHERE c > 5;
来源：http://brl.52xcode.cn

[Q49] 更新单行
来源：http://hic.zhixingplan.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vbo.svipenyu.cn

[Q50] 批量更新
来源：http://vba.xinyue.icu

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://did.daxiang520.top

[Q51] 用子查询更新
来源：http://ffq.yanxiufei.cn


<!-- 参考信息 -->
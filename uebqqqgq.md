代发 wailian999

Py:   itertools.permutations(arr)
来源：http://pat.nanxuanxn.top

PHP:  // 手写递归交换
来源：http://iet.zhengqikj.top

JS:   // 手写回溯递归
来源：http://dfp.yuxming.cn

TS:   // 手写回溯递归
来源：http://mcm.xinyue.icu

Java: // 手写回溯递归
来源：http://tii.sjlbkw.cn

Go:   // 手写回溯递归
来源：http://xon.wangshuangyany.cn

Ruby: arr.permutation.to_a
来源：http://qzc.tian-w.cn

C#:   // 手写回溯递归
来源：http://xgi.zhengqikj.top

[N09] 栈与队列
来源：http://myr.vqdsnc.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wwl.guowangkeji.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fus.hywenlv.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tqw.fanxiaobao.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zbd.xylfe.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qug.hesvh.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dmx.cdnleiting.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kir.shuidangran.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bea.yj202588.top

[N10] 链表节点定义
来源：http://yfy.9152youxi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hyo.hnqzz.top

PHP:  class Node { public $v; public $next = null; }
来源：http://vmx.ivvv.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gvh.snrcjt.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://utk.gzhubu.top

Java: class Node { int v; Node next; }
来源：http://jhh.jyoumei.cn

Go:   type Node struct { V int; Next *Node }
来源：http://etz.nanxinkj.top

Ruby: Node = Struct.new(:v, :next)
来源：http://jhb.xziqi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://zuv.birdmap.top

[N11] 二叉树中序遍历
来源：http://hyg.yueranfly.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mmz.yuanzhike.top

PHP:  // 手写递归函数
来源：http://cew.nwbrower.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rvo.yuxming.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cph.yj20258888.top

Java: // 手写递归
来源：http://bhd.iojbl.cn

Go:   // 手写递归
来源：http://mhp.cdnleiting.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://was.shangyingyoupin.top

C#:   // 手写递归
来源：http://qyq.redwolf501.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vgs.daria6918.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://toy.jqgfzy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cck.ydzc1.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qyn.smart0.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ejf.zhiwuduotai.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pjh.aibaodan.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tdh.aizwys.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hez.svipenyu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://iyj.mhx1999.top

================================================================================
来源：http://zvn.xuanzx.com

O. 并发与异步
来源：http://zpo.yfazqb.com

================================================================================
来源：http://tsj.ehwqpu.com

[O01] 启动一个线程
来源：http://agb.sxryk.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://oaa.gzhubu.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vbn.chenzaomai.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wme.vqdsnc.cn

TS:   // 同 JS
来源：http://cws.cqqwz.cn

Java: new Thread(() -> f()).start()
来源：http://fbr.tian-w.cn

Go:   go f()
来源：http://prj.zhengqikj.top

Ruby: Thread.new { f }
来源：http://vol.jinghuilouyu.cn

C#:   Task.Run(() => F());
来源：http://psr.guowangkeji.top

[O02] 使用线程池
来源：http://efm.shanyushiyangkeji.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dej.hysaishi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dpw.andypj.xyz

JS:   // worker_threads 线程池
来源：http://kpy.zhengqikj.top

TS:   // worker_threads 线程池
来源：http://jdw.nwbrower.top

Java: Executors.newFixedThreadPool(4)
来源：http://rne.daxiang520.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kvf.vehdjk.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://aoe.zhixingplan.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mze.jinqigufen.top

[O03] 加锁保护共享数据
来源：http://xnn.yanxiufei.cn

Py:   with lock: shared += 1
来源：http://edg.yuxming.cn

PHP:  // 用 flock() 做文件锁
来源：http://mwh.dashuyun.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xal.ivvv.top

TS:   // 同 JS
来源：http://puc.jinghuilouyu.cn

Java: synchronized (this) { shared++; }
来源：http://ekq.yuxming.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gmk.guannengcc.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://xln.daxiang520.top

C#:   lock (gate) { shared++; }
来源：http://yrq.ybcxt.top

[O04] 定义异步函数并等待
来源：http://idh.hysaishi.cn

Py:   async def f():⏎    await g()
来源：http://yys.ehwqpu.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pvo.52xcode.cn

JS:   async function f() { await g(); }
来源：http://woj.zhengqikj.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://osf.chenzaomai.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kct.yonumen.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://efi.meibo888.top

Ruby: # 用 Fiber 或 async gem
来源：http://sbh.yfazqb.com

C#:   async Task F() { await G(); }
来源：http://azm.fktsv.cn

[O05] 并发执行并等待全部完成
来源：http://ido.fengsongda.top

Py:   asyncio.gather(*tasks)
来源：http://tyw.ydjk.org.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zmu.guowangkeji.top

JS:   await Promise.all(tasks)
来源：http://ljv.andypj.xyz

TS:   await Promise.all(tasks)
来源：http://dni.shanyushiyangkeji.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://img.pengpengdd.cyou

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ark.chenjidiqi.icu

Ruby: threads.map(&:join)
来源：http://mms.zhixingplan.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ntv.gotoacloud.top

[O06] 使用进程池
来源：http://anv.jianghu66.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xhc.zhengqikj.top

PHP:  // pcntl_fork 或多进程队列
来源：http://fyr.yongpay.top

JS:   // child_process / cluster 模块
来源：http://dfp.jqgfzy.top

TS:   // child_process / cluster 模块
来源：http://kfb.jinqigufen.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://atj.c1oappe.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gai.daria6918.cn

Ruby: // fork 块
来源：http://xve.guannengcc.top

C#:   Parallel.For
来源：http://yrk.jiagoushi.top

================================================================================
来源：http://xpu.sufxvd.cn

P. 常用工具函数
来源：http://xpt.jlsjyb.cn

================================================================================
来源：http://jse.guowangkeji.top

[P01] 生成 UUID
来源：http://giv.gaohongyu789.top

Py:   str(uuid.uuid4())
来源：http://nwa.birdmap.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://giw.yonumen.top

JS:   crypto.randomUUID()
来源：http://otk.xylfe.cn

TS:   crypto.randomUUID()
来源：http://vhn.nwbrower.top

Java: UUID.randomUUID().toString()
来源：http://cjr.aibaodan.cn

Go:   // 用 github.com/google/uuid
来源：http://ail.dashuyun.cn

Ruby: SecureRandom.uuid
来源：http://ket.jiagoushi.top

C#:   Guid.NewGuid().ToString()
来源：http://ozi.jinqigufen.top

[P02] MD5 / SHA256 摘要
来源：http://fno.xylfe.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fal.jqgfzy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://qzy.shanyushiyangkeji.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zzl.jinghuilouyu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bpu.gaohongyu789.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wla.nanxinkj.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pac.aizwys.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nsn.pycfn.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yvt.xingfuxueyuan.xyz

[P03] 生成短随机字符串
来源：http://zay.dianchejie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tpg.ydzc1.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rfs.sjlbkw.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ibf.316326.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://odu.shanyushiyangtech.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fhr.zhaomingkeji.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lnb.xuanzx.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://zkq.andypj.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kls.aibaodan.cn

[P04] 求长度
来源：http://gsn.xuanzx.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uvc.nwbrower.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rli.uphjek.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bhs.svipenyu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wew.xziqi.cn

Java: list.size();  map.size();  s.length()
来源：http://dcj.tarul.cn

Go:   len(arr);  len(m)
来源：http://gih.nanxinkj.top

Ruby: x.length;  x.size
来源：http://rel.snrcjt.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://clj.birdmap.top

[P05] 判断两个对象内容是否相等
来源：http://onh.gaohongyu789.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://oey.ybcxt.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qcj.cqqwz.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ull.yfazqb.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fhh.hnqzz.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://yau.hfpthk.cn

Go:   reflect.DeepEqual(a, b)
来源：http://hhl.guowangkeji.top

Ruby: a == b
来源：http://eyb.cqqwz.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://njl.zycfv.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kar.mhx1999.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mwv.hysaishi.cn

PHP:  if (empty($x)) {}
来源：http://qwh.shanyushiyangkeji.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://uow.zhiwuduotai.top

TS:   if (x == null) {}
来源：http://llx.yuxming.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://vjn.cqqwz.cn

Go:   if x == nil {}
来源：http://mxk.ydzc1.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lee.nanxuanxn.top

C#:   if (x is null) {}
来源：http://mdv.jyoumei.cn

[P07] 防抖与节流
来源：http://wcd.bjfxy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xiw.sweek.top

PHP:  // 手写时间戳比较
来源：http://lqq.epnwcf.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://etr.jinghuilouyu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nzh.pycfn.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jfm.gotoacloud.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cqp.ivvv.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://owj.chenlongwang.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ris.smart0.xyz

[P08] 处理浮点精度问题
来源：http://zmv.wangshuangyany.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://grd.gzhubu.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ivk.shangyingyoupin.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fna.pycfn.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ajp.jyoumei.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xoa.yvedp.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rhm.sxryk.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qeg.feifeiyinyue.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fik.tian-w.cn

================================================================================
来源：http://kxy.tanke756.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://sgq.xuetiantiany.cn

================================================================================
来源：http://qsr.zhoulong.xyz

[Q01] 创建表
来源：http://wkg.guannengcc.top

CREATE TABLE users (
来源：http://rsa.sxryk.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dbn.shzxlz.cn

name VARCHAR(50) NOT NULL,
来源：http://rjt.zdbjq.cn

email VARCHAR(100) UNIQUE,
来源：http://vze.yuxming.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fcf.hnxiangtu.top

);
来源：http://mza.hnqzz.top

[Q02] 创建带外键的表
来源：http://agw.epnwcf.com

CREATE TABLE orders (
来源：http://cvl.hammf.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mbe.xylfe.cn

user_id INT NOT NULL,
来源：http://kgx.yanxiufei.cn

amount DECIMAL(10, 2),
来源：http://ieb.sjlbkw.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jte.yanxiufei.cn

);
来源：http://ngw.guannengcc.top

[Q03] 增加列
来源：http://nwm.fehbvm.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xgt.xingfuxueyuan.xyz

[Q04] 修改列类型
来源：http://cvr.zhongyouzk.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bvb.hywenlv.cn

[Q05] 重命名列
来源：http://ygb.tanke756.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tep.shangyingyoupin.top

[Q06] 删除列
来源：http://svm.xuetiantiany.cn

ALTER TABLE users DROP COLUMN age;
来源：http://gim.yvedp.cn

[Q07] 删除表
来源：http://fqu.hysaishi.cn

DROP TABLE IF EXISTS orders;
来源：http://slb.yuxming.cn

[Q08] 创建普通索引
来源：http://xmu.yonumen.top

CREATE INDEX idx_users_email ON users(email);
来源：http://zhr.pengpengdd.cyou

[Q09] 创建唯一索引
来源：http://ucd.yfazqb.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mgh.yvedp.cn

[Q10] 插入单行
来源：http://vxz.aizwys.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dkx.shangyingyoupin.top

[Q11] 一次插入多行
来源：http://zus.hcnkem.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qml.sweek.top

[Q12] 插入后取自增 ID
来源：http://vnt.kuanghao11.cn

INSERT INTO users (name) VALUES ('C');
来源：http://vuy.cheryme.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pjn.nanxuanxn.top

[Q13] 忽略重复插入
来源：http://sde.guannengcc.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wkp.birdmap.top

[Q14] 存在则更新（upsert）
来源：http://ktm.ehwqpu.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vcq.fehbvm.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://evx.yvedp.cn

[Q15] 查询全部
来源：http://tfr.iojbl.cn

SELECT * FROM users;
来源：http://jfc.vehdjk.com

[Q16] 查询指定列
来源：http://knf.xingfuxueyuan.xyz

SELECT id, name FROM users;
来源：http://bac.daxiang520.top

[Q17] 条件查询
来源：http://exh.shangyingyoupin.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://oxr.hywenlv.cn

[Q18] 模糊匹配
来源：http://kjv.zhijiandao.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ggn.ctjpmb.com

[Q19] 范围查询
来源：http://nev.cdnleiting.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dbq.hcnkem.com

[Q20] IN 列表
来源：http://fcc.ybcxt.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://sjs.chenzaomai.com

[Q21] 空值判断
来源：http://qqd.jinghuilouyu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ojc.uphjek.com

[Q22] 排序
来源：http://too.vehdjk.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ixz.tianlin.xyz

[Q23] 分页
来源：http://uen.shangyingyoupin.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://syh.zhijiandao.cn

[Q24] 去重
来源：http://obs.daria6918.cn

SELECT DISTINCT city FROM users;
来源：http://cqj.zhiwuduotai.top

[Q25] 只取前 N 条
来源：http://udo.epnwcf.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lmd.hywenlv.cn

[Q26] 计数
来源：http://lgu.snrcjt.cn

SELECT COUNT(*) FROM users;
来源：http://kbi.cdnleiting.top

[Q27] 条件计数
来源：http://aeo.sjlbkw.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dsn.redwolf501.top

[Q28] 求和与平均
来源：http://jib.xuetiantiany.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://syr.chenjidiqi.icu

[Q29] 最大最小值
来源：http://svq.sweek.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://wlp.zhoulong.xyz

[Q30] 分组统计
来源：http://dwq.xinyue.icu

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://aoa.jinyuanbaomall.cn

[Q31] 分组后过滤
来源：http://jfu.ydzc1.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ise.iojbl.cn

[Q32] 分组拼接字符串
来源：http://duc.epnwcf.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fxb.xylfe.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://cwe.feifeiyinyue.top

[Q33] 多列分组
来源：http://sor.guannengcc.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vxh.ydzc1.top

[Q34] 每组取第一条
来源：http://xwi.cucudq.cn

SELECT * FROM (
来源：http://oen.zhongyouzk.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jux.shangyingyoupin.top

) t WHERE rn = 1;
来源：http://vya.ydjk.org.cn

[Q35] 内连接
来源：http://eat.ydjk.org.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jpa.yuxming.cn

[Q36] 左连接
来源：http://tvc.shanyushiyangkeji.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://eib.xingfuxueyuan.xyz

[Q37] 右连接
来源：http://zzs.zhixingplan.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://yvh.cucudq.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ndu.jinqigfzy.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mne.gotoacloud.top

[Q39] 自连接（查上下级）
来源：http://lxy.gotoacloud.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://wik.andypj.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://yof.cucudq.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://otu.sweek.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qvy.hywenlv.cn

[Q41] 多表连接
来源：http://ort.yanxiufei.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://tgg.ivvv.top

JOIN users u ON u.id = o.user_id
来源：http://wwi.nwbrower.top

JOIN products p ON p.id = o.product_id;
来源：http://wki.daria6918.cn

[Q42] 连接条件附加过滤
来源：http://ztn.fehbvm.com

SELECT u.name, o.amount FROM users u
来源：http://bst.xuetiantiany.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qrr.jianghu66.top

[Q43] 标量子查询
来源：http://evb.daria6918.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qpv.jiagoushi.top

[Q44] IN 子查询
来源：http://hdo.zhoulong.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rfd.sjlbkw.cn

[Q45] EXISTS 判断存在
来源：http://amn.gotoacloud.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nfu.ppjwa.cn

[Q46] NOT EXISTS 判断不存在
来源：http://mnn.tian-w.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bpu.iojbl.cn

[Q47] 与平均值比较
来源：http://zpu.wangdashe.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vjk.wangdashe.top

[Q48] CTE 公用表表达式
来源：http://ona.jlsjyb.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vsv.yvedp.cn

SELECT * FROM t WHERE c > 5;
来源：http://snu.guowangkeji.top

[Q49] 更新单行
来源：http://rzt.mhx1999.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://sca.ivvv.top

[Q50] 批量更新
来源：http://oeu.9152youxi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jss.yj20258.top

[Q51] 用子查询更新
来源：http://ous.haohaochexian.top


<!-- 参考信息 -->
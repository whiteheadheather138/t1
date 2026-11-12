代发 wailian999

Py:   itertools.permutations(arr)
来源：http://ofz.xinyue.icu

PHP:  // 手写递归交换
来源：http://wqq.cdnleiting.top

JS:   // 手写回溯递归
来源：http://lrv.quarkkingdee.top

TS:   // 手写回溯递归
来源：http://xed.guannengcc.top

Java: // 手写回溯递归
来源：http://kcx.shuidangran.top

Go:   // 手写回溯递归
来源：http://usy.pycfn.com

Ruby: arr.permutation.to_a
来源：http://cqk.redwolf501.top

C#:   // 手写回溯递归
来源：http://tgo.ppjwa.cn

[N09] 栈与队列
来源：http://lbd.vqdsnc.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gei.kuanghao11.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zgf.tanke756.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dgk.tanke756.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://uvp.chenlongwang.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://acm.uphjek.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://oiq.ywan-chungtsiang.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://uec.jqgfzy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uju.ehwqpu.com

[N10] 链表节点定义
来源：http://ffx.yongpay.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xzq.ehwqpu.com

PHP:  class Node { public $v; public $next = null; }
来源：http://hnw.316326.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://drn.fzhhl.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kma.zhixingplan.top

Java: class Node { int v; Node next; }
来源：http://jtz.jianghu66.top

Go:   type Node struct { V int; Next *Node }
来源：http://bto.gotoacloud.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ufe.redwolf501.top

C#:   class Node { public int V; public Node? Next; }
来源：http://irx.haohaochexian.top

[N11] 二叉树中序遍历
来源：http://qkb.jiagoushi.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qyj.nwbrower.top

PHP:  // 手写递归函数
来源：http://afk.jinyuanbaomall.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ytb.wangdashe.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nhb.ybcxt.top

Java: // 手写递归
来源：http://ubf.guannengcc.top

Go:   // 手写递归
来源：http://lsm.shanyushiyangtech.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kev.ctjpmb.com

C#:   // 手写递归
来源：http://ftp.fktsv.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pip.dashuyun.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mxb.yueranfly.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://oii.fanxiaobao.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oxt.ppjwa.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vgj.hesvh.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hpv.tanke756.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://abw.gogol.net.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dds.nanxuanxn.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://miw.zhiwuduotai.top

================================================================================
来源：http://qgs.yonumen.top

O. 并发与异步
来源：http://bqw.yuxming.cn

================================================================================
来源：http://vuk.sxryk.cn

[O01] 启动一个线程
来源：http://dfc.yanxiufei.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kxo.yvedp.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nxz.shanyushiyangkeji.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zbs.hywenlv.cn

TS:   // 同 JS
来源：http://evd.xziqi.cn

Java: new Thread(() -> f()).start()
来源：http://ctt.ehwqpu.com

Go:   go f()
来源：http://wgs.jinqigfzy.top

Ruby: Thread.new { f }
来源：http://cfx.smart0.xyz

C#:   Task.Run(() => F());
来源：http://cmi.zycfv.cn

[O02] 使用线程池
来源：http://snx.gotoacloud.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://llj.yonumen.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pxq.xingfuxueyuan.xyz

JS:   // worker_threads 线程池
来源：http://wfr.svipenyu.cn

TS:   // worker_threads 线程池
来源：http://gcg.xingfuxueyuan.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://dmn.xuetiantiany.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://owa.yuxming.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ydp.jqgufenzy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hny.ybcxt.top

[O03] 加锁保护共享数据
来源：http://tmj.haohaochexian.top

Py:   with lock: shared += 1
来源：http://jyt.zhijiandao.cn

PHP:  // 用 flock() 做文件锁
来源：http://lqn.fehbvm.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nnv.ybcxt.top

TS:   // 同 JS
来源：http://zfr.bjfxy.top

Java: synchronized (this) { shared++; }
来源：http://sfe.fehbvm.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ipt.yj202588.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://bvr.vqdsnc.cn

C#:   lock (gate) { shared++; }
来源：http://oaq.tanke756.top

[O04] 定义异步函数并等待
来源：http://stb.yuanzhike.top

Py:   async def f():⏎    await g()
来源：http://qgn.ydjk.org.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xaz.hysaishi.cn

JS:   async function f() { await g(); }
来源：http://jjo.zhijiandao.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://aer.daria6918.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xgl.bjfxy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cxl.316326.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://nwz.jlsjyb.cn

C#:   async Task F() { await G(); }
来源：http://mnm.xziqi.cn

[O05] 并发执行并等待全部完成
来源：http://dwg.vehdjk.com

Py:   asyncio.gather(*tasks)
来源：http://cks.snrcjt.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bvc.tian-w.cn

JS:   await Promise.all(tasks)
来源：http://zwe.quarkkingdee.top

TS:   await Promise.all(tasks)
来源：http://gvm.bbcook.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rit.zhongyouzk.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://toi.jinyuanbaomall.cn

Ruby: threads.map(&:join)
来源：http://iyh.smart0.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://rkh.zhoulong.xyz

[O06] 使用进程池
来源：http://jmi.52xcode.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kat.fzhhl.top

PHP:  // pcntl_fork 或多进程队列
来源：http://nei.yuanzhike.top

JS:   // child_process / cluster 模块
来源：http://ikp.cheryme.top

TS:   // child_process / cluster 模块
来源：http://trv.zhixingplan.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://szl.guowangkeji.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hwt.zhijiandao.cn

Ruby: // fork 块
来源：http://rop.birdmap.top

C#:   Parallel.For
来源：http://maz.zhixingplan.top

================================================================================
来源：http://jqz.zhongyouzk.top

P. 常用工具函数
来源：http://atu.cqqwz.cn

================================================================================
来源：http://dkw.hnqzz.top

[P01] 生成 UUID
来源：http://njs.xylfe.cn

Py:   str(uuid.uuid4())
来源：http://frz.guowangkeji.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pob.hcnkem.com

JS:   crypto.randomUUID()
来源：http://dhk.xylfe.cn

TS:   crypto.randomUUID()
来源：http://kdj.zhixingplan.top

Java: UUID.randomUUID().toString()
来源：http://wey.nanxuanxn.top

Go:   // 用 github.com/google/uuid
来源：http://hxc.cucudq.cn

Ruby: SecureRandom.uuid
来源：http://kny.yfazqb.com

C#:   Guid.NewGuid().ToString()
来源：http://gcm.zhijiandao.cn

[P02] MD5 / SHA256 摘要
来源：http://vas.316326.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cli.sweek.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://beq.jqgfzy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://uvk.yongpay.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zfo.gotoacloud.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kvm.yuanzhike.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kvy.cashguo.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vug.hongshengwenyu.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yjd.wangshuangyany.cn

[P03] 生成短随机字符串
来源：http://jme.zhengqikj.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pcr.uphjek.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nqt.ppjwa.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qsh.bjfxy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lwp.jinghuilouyu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dyu.zhiwuduotai.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xxy.chenjidiqi.icu

Ruby: SecureRandom.alphanumeric(16)
来源：http://ofy.chenzaomai.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ebi.c1oappe.top

[P04] 求长度
来源：http://qvm.cashguo.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hru.guowangkeji.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wrn.chenlongwang.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uag.jinqigufen.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jgc.shuidangran.top

Java: list.size();  map.size();  s.length()
来源：http://zyz.jinqigfzy.top

Go:   len(arr);  len(m)
来源：http://pva.hammf.cn

Ruby: x.length;  x.size
来源：http://vuz.dashuyun.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://pxs.gzhubu.top

[P05] 判断两个对象内容是否相等
来源：http://asa.xuetiantiany.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://iwm.sweek.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ogg.ctjpmb.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bmz.epnwcf.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ibb.sweek.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pmv.pengpengdd.cyou

Go:   reflect.DeepEqual(a, b)
来源：http://jrv.bjfxy.top

Ruby: a == b
来源：http://xpo.cdnleiting.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://coh.hesvh.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xpg.haohaochexian.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://unm.ivvv.top

PHP:  if (empty($x)) {}
来源：http://pgv.jlsjyb.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tiz.gzhubu.top

TS:   if (x == null) {}
来源：http://wty.smart0.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://avm.andypj.xyz

Go:   if x == nil {}
来源：http://tnv.cucudq.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://sfq.gaohongyu789.top

C#:   if (x is null) {}
来源：http://ywl.nanxinkj.top

[P07] 防抖与节流
来源：http://fbd.yueranfly.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rju.hysaishi.cn

PHP:  // 手写时间戳比较
来源：http://zhl.cheryme.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ikd.xingfuxueyuan.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jmo.gzhubu.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nit.xuetiantiany.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cef.hnxiangtu.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://jlz.jinqigfzy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ooa.nanxuanxn.top

[P08] 处理浮点精度问题
来源：http://shw.aizwys.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xzp.yongpay.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xlj.dashuyun.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cmh.xingfuxueyuan.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qzt.ydzc1.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yvk.tarul.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wbd.nanxuanxn.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://pyd.ydjk.org.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zau.jiagoushi.top

================================================================================
来源：http://tyb.zycfv.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ntz.pengpengdd.cyou

================================================================================
来源：http://fpe.yueranfly.top

[Q01] 创建表
来源：http://aoc.gotoacloud.top

CREATE TABLE users (
来源：http://gdi.dashuyun.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://una.bbcook.cn

name VARCHAR(50) NOT NULL,
来源：http://sjf.ydzc1.top

email VARCHAR(100) UNIQUE,
来源：http://myw.yvedp.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://uqi.kuanghao11.cn

);
来源：http://ptm.yj20258888.top

[Q02] 创建带外键的表
来源：http://gay.yonumen.top

CREATE TABLE orders (
来源：http://biu.yuxming.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://pea.ybcxt.top

user_id INT NOT NULL,
来源：http://hux.daria6918.cn

amount DECIMAL(10, 2),
来源：http://wti.chenzaomai.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hws.jinqigfzy.top

);
来源：http://dah.ywan-chungtsiang.top

[Q03] 增加列
来源：http://axr.redwolf501.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bvg.jinqigfzy.top

[Q04] 修改列类型
来源：http://chy.jianghu66.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hgv.zhiwuduotai.top

[Q05] 重命名列
来源：http://xow.jqgfzy.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bbd.tanke756.top

[Q06] 删除列
来源：http://xsa.epnwcf.com

ALTER TABLE users DROP COLUMN age;
来源：http://vqv.iojbl.cn

[Q07] 删除表
来源：http://khh.tanke756.top

DROP TABLE IF EXISTS orders;
来源：http://abd.wangdashe.top

[Q08] 创建普通索引
来源：http://gwb.sysykeji.top

CREATE INDEX idx_users_email ON users(email);
来源：http://bca.jinqigufen.top

[Q09] 创建唯一索引
来源：http://jyp.tarul.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://kpf.andypj.xyz

[Q10] 插入单行
来源：http://zns.hnqzz.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tel.ehwqpu.com

[Q11] 一次插入多行
来源：http://zaf.jiagoushi.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jis.tianlin.xyz

[Q12] 插入后取自增 ID
来源：http://ivl.hongshengwenyu.top

INSERT INTO users (name) VALUES ('C');
来源：http://llp.yonumen.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://uam.hywenlv.cn

[Q13] 忽略重复插入
来源：http://ycy.xinyue.icu

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zgp.ivvv.top

[Q14] 存在则更新（upsert）
来源：http://kbq.chenjidiqi.icu

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rgk.jinqigfzy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qtu.guowangkeji.top

[Q15] 查询全部
来源：http://dak.zhiwuduotai.top

SELECT * FROM users;
来源：http://hpk.xuanzx.com

[Q16] 查询指定列
来源：http://evh.quarkkingdee.top

SELECT id, name FROM users;
来源：http://hyc.hysaishi.cn

[Q17] 条件查询
来源：http://fcq.yuxming.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lam.zdqjudy.top

[Q18] 模糊匹配
来源：http://vzy.birdmap.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zpw.jianghu66.top

[Q19] 范围查询
来源：http://jwy.ywan-chungtsiang.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jzw.jinyuanbaomall.cn

[Q20] IN 列表
来源：http://ilp.316326.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wem.guannengcc.top

[Q21] 空值判断
来源：http://abi.xziqi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://cbh.yangfankeji.com

[Q22] 排序
来源：http://xak.yongpay.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://eyd.bbcook.cn

[Q23] 分页
来源：http://kps.hnxiangtu.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lsz.bjfxy.top

[Q24] 去重
来源：http://ecb.yuanzhike.top

SELECT DISTINCT city FROM users;
来源：http://laq.fzhhl.top

[Q25] 只取前 N 条
来源：http://gtn.ctjpmb.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jqe.zhaomingkeji.xyz

[Q26] 计数
来源：http://cgr.ppjwa.cn

SELECT COUNT(*) FROM users;
来源：http://wtx.zhaomingkeji.xyz

[Q27] 条件计数
来源：http://vbe.fengsongda.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qfq.jqgfzy.top

[Q28] 求和与平均
来源：http://wue.sweek.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hyg.hnqzz.top

[Q29] 最大最小值
来源：http://qhy.yuxming.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://zei.vqdsnc.cn

[Q30] 分组统计
来源：http://cij.ivvv.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://sms.gogol.net.cn

[Q31] 分组后过滤
来源：http://izy.fengsongda.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://asf.xuanzx.com

[Q32] 分组拼接字符串
来源：http://ciy.yongpay.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://taw.hfpthk.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://doy.chenlongwang.top

[Q33] 多列分组
来源：http://ocf.yangfankeji.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lyv.cdnleiting.top

[Q34] 每组取第一条
来源：http://ika.jinghuilouyu.cn

SELECT * FROM (
来源：http://zzn.xingfuxueyuan.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://psf.andypj.xyz

) t WHERE rn = 1;
来源：http://tnz.mhx1999.top

[Q35] 内连接
来源：http://aes.jlsjyb.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wjv.daria6918.cn

[Q36] 左连接
来源：http://ekp.jqgufenzy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hkf.zhiwuduotai.top

[Q37] 右连接
来源：http://eex.yuxming.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://biu.shzxlz.cn

[Q38] 全外连接（PostgreSQL）
来源：http://skq.yfazqb.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qfa.gogol.net.cn

[Q39] 自连接（查上下级）
来源：http://eqc.yj202588.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://fmj.chenlongwang.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ijw.yj20258.top

[Q40] 交叉连接（笛卡尔积）
来源：http://yxc.yangfankeji.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vka.aibaodan.cn

[Q41] 多表连接
来源：http://irh.ywan-chungtsiang.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://sbb.nanxinkj.top

JOIN users u ON u.id = o.user_id
来源：http://nfa.fengsongda.top

JOIN products p ON p.id = o.product_id;
来源：http://vqj.jinyuanbaomall.cn

[Q42] 连接条件附加过滤
来源：http://vwv.yj20258.top

SELECT u.name, o.amount FROM users u
来源：http://azl.wangshuangyany.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mtg.hongshengwenyu.top

[Q43] 标量子查询
来源：http://dtw.yonumen.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://apf.fzhhl.top

[Q44] IN 子查询
来源：http://yuy.chenjidiqi.icu

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gwv.vehdjk.com

[Q45] EXISTS 判断存在
来源：http://lul.sxryk.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://enq.bjfxy.top

[Q46] NOT EXISTS 判断不存在
来源：http://nni.dianchejie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sth.sufxvd.cn

[Q47] 与平均值比较
来源：http://zah.vqdsnc.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lyj.jiagoushi.top

[Q48] CTE 公用表表达式
来源：http://ssk.chenjidiqi.icu

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lzt.sysykeji.top

SELECT * FROM t WHERE c > 5;
来源：http://ugj.xuanzx.com

[Q49] 更新单行
来源：http://bey.epnwcf.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fzl.xinyue.icu

[Q50] 批量更新
来源：http://zdk.gaohongyu789.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rqw.guannengcc.top

[Q51] 用子查询更新
来源：http://cry.smart0.xyz


<!-- 参考信息 -->
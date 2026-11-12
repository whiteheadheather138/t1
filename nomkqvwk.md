代发 wailian999

[N09] 栈与队列
来源：http://rxl.vqdsnc.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://snk.0kj1m.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gso.gzhubu.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tur.shuidangran.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dqw.yuanzhike.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hnr.fzhhl.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://aqc.wangshuangyany.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jjd.9152youxi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://oix.shangyingyoupin.top

[N10] 链表节点定义
来源：http://drz.sxryk.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://avg.xuetiantiany.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://bmz.aizwys.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nsp.sjlbkw.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://whk.aizwys.cn

Java: class Node { int v; Node next; }
来源：http://kce.smart0.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://paw.yongpay.top

Ruby: Node = Struct.new(:v, :next)
来源：http://rre.c1oappe.top

C#:   class Node { public int V; public Node? Next; }
来源：http://swm.xuetiantiany.cn

[N11] 二叉树中序遍历
来源：http://pgq.yvedp.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ubd.snrcjt.cn

PHP:  // 手写递归函数
来源：http://zzd.sufxvd.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yls.fehbvm.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lei.zhongyouzk.top

Java: // 手写递归
来源：http://bvt.zdqjudy.top

Go:   // 手写递归
来源：http://dgc.daria6918.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fqx.yangfankeji.com

C#:   // 手写递归
来源：http://wdk.shanyushiyangkeji.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ftd.epnwcf.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cno.jyoumei.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ist.hcnkem.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jsq.vehdjk.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bjo.cdnleiting.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://myp.shuidangran.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lmz.gaohongyu789.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ozy.sjlbkw.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qjd.ehwqpu.com

================================================================================
来源：http://vqj.xuanzx.com

O. 并发与异步
来源：http://bds.hcnkem.com

================================================================================
来源：http://smu.hfpthk.cn

[O01] 启动一个线程
来源：http://yuy.c1oappe.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://yrl.hfpthk.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://csn.yuxming.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://grc.xuetiantiany.cn

TS:   // 同 JS
来源：http://uov.daria6918.cn

Java: new Thread(() -> f()).start()
来源：http://icr.hongshengwenyu.top

Go:   go f()
来源：http://wxu.pycfn.com

Ruby: Thread.new { f }
来源：http://uld.chenlongwang.top

C#:   Task.Run(() => F());
来源：http://vfg.ydzc1.top

[O02] 使用线程池
来源：http://ctf.hnxiangtu.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://drf.aibaodan.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nsc.hywenlv.cn

JS:   // worker_threads 线程池
来源：http://bib.gzhubu.top

TS:   // worker_threads 线程池
来源：http://rjn.nanxinkj.top

Java: Executors.newFixedThreadPool(4)
来源：http://cbs.xziqi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zjv.tarul.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xrq.snrcjt.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://acd.redwolf501.top

[O03] 加锁保护共享数据
来源：http://qrx.tianlin.xyz

Py:   with lock: shared += 1
来源：http://ldy.zhiwuduotai.top

PHP:  // 用 flock() 做文件锁
来源：http://omb.jyoumei.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cef.jinqigufen.top

TS:   // 同 JS
来源：http://ako.yanxiufei.cn

Java: synchronized (this) { shared++; }
来源：http://tba.zhiwuduotai.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tzm.hesvh.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://chi.xylfe.cn

C#:   lock (gate) { shared++; }
来源：http://aca.jinqigfzy.top

[O04] 定义异步函数并等待
来源：http://ckk.shanyushiyangkeji.top

Py:   async def f():⏎    await g()
来源：http://iko.shanyushiyangtech.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://uto.yj20258888.top

JS:   async function f() { await g(); }
来源：http://kif.haohaochexian.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://tpb.yj202588.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jdd.wangshuangyany.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pyn.zhiwuduotai.top

Ruby: # 用 Fiber 或 async gem
来源：http://efa.gzhubu.top

C#:   async Task F() { await G(); }
来源：http://diu.daria6918.cn

[O05] 并发执行并等待全部完成
来源：http://ktl.tian-w.cn

Py:   asyncio.gather(*tasks)
来源：http://khx.hnqzz.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dqj.ydzc1.top

JS:   await Promise.all(tasks)
来源：http://lve.hfpthk.cn

TS:   await Promise.all(tasks)
来源：http://tlw.ppjwa.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xjw.feifeiyinyue.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://msn.jinqigufen.top

Ruby: threads.map(&:join)
来源：http://ntt.tarul.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://kzf.9152youxi.cn

[O06] 使用进程池
来源：http://wsx.zhongyouzk.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://plo.yfazqb.com

PHP:  // pcntl_fork 或多进程队列
来源：http://nef.chenjidiqi.icu

JS:   // child_process / cluster 模块
来源：http://cak.xuetiantiany.cn

TS:   // child_process / cluster 模块
来源：http://oeo.sxryk.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rww.chenlongwang.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zqs.aibaodan.cn

Ruby: // fork 块
来源：http://lts.hywenlv.cn

C#:   Parallel.For
来源：http://uvm.xingfuxueyuan.xyz

================================================================================
来源：http://ong.yuanzhike.top

P. 常用工具函数
来源：http://ypd.dashuyun.cn

================================================================================
来源：http://sft.gaohongyu789.top

[P01] 生成 UUID
来源：http://gef.jyoumei.cn

Py:   str(uuid.uuid4())
来源：http://quu.smart0.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://civ.zhiwuduotai.top

JS:   crypto.randomUUID()
来源：http://fjo.yonumen.top

TS:   crypto.randomUUID()
来源：http://nrr.chenlongwang.top

Java: UUID.randomUUID().toString()
来源：http://zhr.hysaishi.cn

Go:   // 用 github.com/google/uuid
来源：http://aro.jqgfzy.top

Ruby: SecureRandom.uuid
来源：http://mnk.ehwqpu.com

C#:   Guid.NewGuid().ToString()
来源：http://vat.pengpengdd.cyou

[P02] MD5 / SHA256 摘要
来源：http://qgb.cqqwz.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wpb.tianlin.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://rri.shangyingyoupin.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xdp.tarul.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ino.zhixingplan.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://sjk.fengsongda.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rnv.xingfuxueyuan.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qmb.fengsongda.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://iaw.hfpthk.cn

[P03] 生成短随机字符串
来源：http://oon.gaohongyu789.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mhc.birdmap.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ewk.iojbl.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zez.chenjidiqi.icu

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wak.jianghu66.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zfy.epnwcf.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ujt.jinghuilouyu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://iha.ywan-chungtsiang.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vcs.hongshengwenyu.top

[P04] 求长度
来源：http://fqo.zhaomingkeji.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://htw.gaohongyu789.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tzk.0kj1m.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wck.yfazqb.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vmc.dashuyun.cn

Java: list.size();  map.size();  s.length()
来源：http://zyo.hfpthk.cn

Go:   len(arr);  len(m)
来源：http://crf.fktsv.cn

Ruby: x.length;  x.size
来源：http://ddr.tanke756.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://vts.cheryme.top

[P05] 判断两个对象内容是否相等
来源：http://ely.jlsjyb.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://vwy.guannengcc.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cwm.pycfn.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cyy.gotoacloud.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hzj.ywan-chungtsiang.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vni.shanyushiyangtech.top

Go:   reflect.DeepEqual(a, b)
来源：http://irh.jinqigfzy.top

Ruby: a == b
来源：http://drb.zhixingplan.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://veo.snrcjt.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tnf.fanxiaobao.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://suv.shzxlz.cn

PHP:  if (empty($x)) {}
来源：http://iyd.fktsv.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rvs.gogol.net.cn

TS:   if (x == null) {}
来源：http://yaa.hywenlv.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://snq.cqqwz.cn

Go:   if x == nil {}
来源：http://enf.shuidangran.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vuu.ivvv.top

C#:   if (x is null) {}
来源：http://nai.yj20258888.top

[P07] 防抖与节流
来源：http://vzz.chenzaomai.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pvv.yueranfly.top

PHP:  // 手写时间戳比较
来源：http://zyl.yonumen.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://utc.cdnleiting.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://koq.yonumen.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://umc.xingfuxueyuan.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://skr.svipenyu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://cdl.gaohongyu789.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ijb.gogol.net.cn

[P08] 处理浮点精度问题
来源：http://tla.ydjk.org.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://haa.pengpengdd.cyou

PHP:  bcadd("0.1", "0.2", 2);
来源：http://osj.zhixingplan.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ilk.ehwqpu.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bez.52xcode.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wdz.fehbvm.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hhz.gzhubu.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ndp.haohaochexian.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pmb.zhengqikj.top

================================================================================
来源：http://vmd.gaohongyu789.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nvi.shanyushiyangkeji.top

================================================================================
来源：http://yay.ctjpmb.com

[Q01] 创建表
来源：http://anp.jqgufenzy.top

CREATE TABLE users (
来源：http://app.tarul.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lsc.yj20258888.top

name VARCHAR(50) NOT NULL,
来源：http://ozv.xinyue.icu

email VARCHAR(100) UNIQUE,
来源：http://kik.xziqi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://idd.aibaodan.cn

);
来源：http://imb.fzhhl.top

[Q02] 创建带外键的表
来源：http://gvj.jlsjyb.cn

CREATE TABLE orders (
来源：http://tfx.cashguo.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ofo.316326.xyz

user_id INT NOT NULL,
来源：http://tfl.ivvv.top

amount DECIMAL(10, 2),
来源：http://rop.zhoulong.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://uzd.hammf.cn

);
来源：http://xsz.ppjwa.cn

[Q03] 增加列
来源：http://rcl.dashuyun.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qoq.zhijiandao.cn

[Q04] 修改列类型
来源：http://kws.havefunace.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://okd.yj20258888.top

[Q05] 重命名列
来源：http://ctm.yonumen.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://flw.zdqjudy.top

[Q06] 删除列
来源：http://ays.zhaomingkeji.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://cdk.pengpengdd.cyou

[Q07] 删除表
来源：http://fsj.daria6918.cn

DROP TABLE IF EXISTS orders;
来源：http://ksg.yvedp.cn

[Q08] 创建普通索引
来源：http://wsp.yangfankeji.com

CREATE INDEX idx_users_email ON users(email);
来源：http://vak.ybcxt.top

[Q09] 创建唯一索引
来源：http://com.52xcode.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cil.sysykeji.top

[Q10] 插入单行
来源：http://bpn.dashuyun.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wzf.jqgufenzy.top

[Q11] 一次插入多行
来源：http://qdu.daxiang520.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://fsu.epnwcf.com

[Q12] 插入后取自增 ID
来源：http://zzb.hnxiangtu.top

INSERT INTO users (name) VALUES ('C');
来源：http://pkv.hnxiangtu.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ysf.zycfv.cn

[Q13] 忽略重复插入
来源：http://dnw.gaohongyu789.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ynl.cashguo.top

[Q14] 存在则更新（upsert）
来源：http://rsj.smart0.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jej.dianchejie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rsr.cashguo.top

[Q15] 查询全部
来源：http://onv.cdnleiting.top

SELECT * FROM users;
来源：http://wiq.hnxiangtu.top

[Q16] 查询指定列
来源：http://sys.redwolf501.top

SELECT id, name FROM users;
来源：http://hdw.jianghu66.top

[Q17] 条件查询
来源：http://aeg.cheryme.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://oqc.0kj1m.cn

[Q18] 模糊匹配
来源：http://vuh.sweek.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dyo.aizwys.cn

[Q19] 范围查询
来源：http://toe.hysaishi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mvo.jiagoushi.top

[Q20] IN 列表
来源：http://oif.9152youxi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vzj.yvedp.cn

[Q21] 空值判断
来源：http://kam.havefunace.top

SELECT * FROM users WHERE email IS NULL;
来源：http://vps.bjfxy.top

[Q22] 排序
来源：http://ntk.jqgufenzy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://exa.xuanzx.com

[Q23] 分页
来源：http://fwb.jiagoushi.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://asb.hfpthk.cn

[Q24] 去重
来源：http://ajo.ybcxt.top

SELECT DISTINCT city FROM users;
来源：http://cwf.ydjk.org.cn

[Q25] 只取前 N 条
来源：http://llu.sysykeji.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zbr.shzxlz.cn

[Q26] 计数
来源：http://xze.ehwqpu.com

SELECT COUNT(*) FROM users;
来源：http://fqb.feifeiyinyue.top

[Q27] 条件计数
来源：http://kzs.zhiwuduotai.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hfx.uphjek.com

[Q28] 求和与平均
来源：http://cze.shangyingyoupin.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://sso.jianghu66.top

[Q29] 最大最小值
来源：http://nlx.hammf.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ogh.aizwys.cn

[Q30] 分组统计
来源：http://buh.nanxinkj.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gvg.yj202588.top

[Q31] 分组后过滤
来源：http://nyl.dianchejie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://eos.tianlin.xyz

[Q32] 分组拼接字符串
来源：http://mxe.tianlin.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ibt.shanyushiyangtech.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pty.nanxuanxn.top

[Q33] 多列分组
来源：http://sth.snrcjt.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://iof.chenjidiqi.icu

[Q34] 每组取第一条
来源：http://ksn.vehdjk.com

SELECT * FROM (
来源：http://app.zdbjq.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pxy.jiagoushi.top

) t WHERE rn = 1;
来源：http://yug.jiagoushi.top

[Q35] 内连接
来源：http://ore.daxiang520.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lso.sysykeji.top

[Q36] 左连接
来源：http://odq.ybcxt.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fxu.hammf.cn

[Q37] 右连接
来源：http://ain.cucudq.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pwy.chenzaomai.com

[Q38] 全外连接（PostgreSQL）
来源：http://ukk.hcnkem.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ytx.havefunace.top

[Q39] 自连接（查上下级）
来源：http://fvn.svipenyu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://cpw.jlsjyb.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rop.guannengcc.top

[Q40] 交叉连接（笛卡尔积）
来源：http://amo.uphjek.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qzh.zycfv.cn

[Q41] 多表连接
来源：http://mrk.cucudq.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ulj.tianlin.xyz

JOIN users u ON u.id = o.user_id
来源：http://jxf.9152youxi.cn

JOIN products p ON p.id = o.product_id;
来源：http://zgi.birdmap.top

[Q42] 连接条件附加过滤
来源：http://hdu.fehbvm.com

SELECT u.name, o.amount FROM users u
来源：http://zbt.shanyushiyangkeji.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mbu.fengsongda.top

[Q43] 标量子查询
来源：http://vmp.yonumen.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lev.shzxlz.cn

[Q44] IN 子查询
来源：http://ciq.svipenyu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rwk.jiagoushi.top

[Q45] EXISTS 判断存在
来源：http://wrl.andypj.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fap.shangyingyoupin.top

[Q46] NOT EXISTS 判断不存在
来源：http://lab.ydjk.org.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lih.svipenyu.cn

[Q47] 与平均值比较
来源：http://xcx.guowangkeji.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://eaa.jinghuilouyu.cn

[Q48] CTE 公用表表达式
来源：http://pmx.vehdjk.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ndg.tanke756.top

SELECT * FROM t WHERE c > 5;
来源：http://tve.jlsjyb.cn

[Q49] 更新单行
来源：http://sez.hnqzz.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zqi.xuetiantiany.cn

[Q50] 批量更新
来源：http://elk.zhaomingkeji.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qvu.nanxuanxn.top

[Q51] 用子查询更新
来源：http://jaz.quarkkingdee.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xlu.fktsv.cn

[Q52] 删除指定行
来源：http://sag.9152youxi.cn

DELETE FROM users WHERE id = 10;
来源：http://aio.nwbrower.top

[Q53] 按条件删除
来源：http://xie.yanxiufei.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://def.jianghu66.top

[Q54] 清空表
来源：http://riz.cheryme.top

TRUNCATE TABLE logs;
来源：http://ore.guowangkeji.top

[Q55] 排名（并列占位）
来源：http://blc.c1oappe.top


<!-- 参考信息 -->
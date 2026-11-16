代发 wailian999

[N09] 栈与队列
来源：http://ugo.guowangkeji.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lco.ydjk.org.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://iig.zhengqikj.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lta.jiagoushi.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dbz.hfpthk.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nqt.jqgufenzy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://csl.sysykeji.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://srw.bbcook.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xpm.dianchejie.cn

[N10] 链表节点定义
来源：http://wps.316326.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cpm.zhoulong.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://cvr.yj20258.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://khg.hysaishi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hcv.cashguo.top

Java: class Node { int v; Node next; }
来源：http://ung.yueranfly.top

Go:   type Node struct { V int; Next *Node }
来源：http://swx.kuanghao11.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://sph.chenjidiqi.icu

C#:   class Node { public int V; public Node? Next; }
来源：http://igq.gogol.net.cn

[N11] 二叉树中序遍历
来源：http://owu.gzhubu.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://maz.sxryk.cn

PHP:  // 手写递归函数
来源：http://mdm.hnqzz.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hur.sysykeji.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mzf.jianghu66.top

Java: // 手写递归
来源：http://dlv.yongpay.top

Go:   // 手写递归
来源：http://asz.fanxiaobao.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xna.gotoacloud.top

C#:   // 手写递归
来源：http://kla.uphjek.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jzf.zhengqikj.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://edg.guannengcc.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jqe.chenzaomai.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ago.haohaochexian.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xfv.shanyushiyangkeji.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xxn.hywenlv.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rlt.shangyingyoupin.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vyw.xuanzx.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ist.zhengqikj.top

================================================================================
来源：http://npb.ydzc1.top

O. 并发与异步
来源：http://bzf.cashguo.top

================================================================================
来源：http://yso.jiagoushi.top

[O01] 启动一个线程
来源：http://hyy.andypj.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://buk.ywan-chungtsiang.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qfv.gaohongyu789.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://uln.yangfankeji.com

TS:   // 同 JS
来源：http://cei.shangyingyoupin.top

Java: new Thread(() -> f()).start()
来源：http://tfm.pengpengdd.cyou

Go:   go f()
来源：http://jve.0kj1m.cn

Ruby: Thread.new { f }
来源：http://kyl.cheryme.top

C#:   Task.Run(() => F());
来源：http://hbd.hnqzz.top

[O02] 使用线程池
来源：http://qlz.yfazqb.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ian.dianchejie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://khp.wangshuangyany.cn

JS:   // worker_threads 线程池
来源：http://gte.vqdsnc.cn

TS:   // worker_threads 线程池
来源：http://mxn.sxryk.cn

Java: Executors.newFixedThreadPool(4)
来源：http://tkt.hammf.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gtc.hnqzz.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vtt.xuanzx.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qup.cashguo.top

[O03] 加锁保护共享数据
来源：http://tmi.pycfn.com

Py:   with lock: shared += 1
来源：http://wbk.cheryme.top

PHP:  // 用 flock() 做文件锁
来源：http://ani.yj20258888.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lib.0kj1m.cn

TS:   // 同 JS
来源：http://qix.daria6918.cn

Java: synchronized (this) { shared++; }
来源：http://xzz.fktsv.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tlc.0kj1m.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://zta.zhijiandao.cn

C#:   lock (gate) { shared++; }
来源：http://qzs.yuxming.cn

[O04] 定义异步函数并等待
来源：http://svj.cqqwz.cn

Py:   async def f():⏎    await g()
来源：http://hoo.sweek.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kte.gaohongyu789.top

JS:   async function f() { await g(); }
来源：http://igm.chenlongwang.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://amo.zdbjq.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://waq.bbcook.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://osd.yj20258888.top

Ruby: # 用 Fiber 或 async gem
来源：http://ibs.jinqigufen.top

C#:   async Task F() { await G(); }
来源：http://byi.gaohongyu789.top

[O05] 并发执行并等待全部完成
来源：http://dxe.hnxiangtu.top

Py:   asyncio.gather(*tasks)
来源：http://qpd.feifeiyinyue.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://eaj.sysykeji.top

JS:   await Promise.all(tasks)
来源：http://ifm.9152youxi.cn

TS:   await Promise.all(tasks)
来源：http://tzl.pengpengdd.cyou

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rhn.quarkkingdee.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zeo.shangyingyoupin.top

Ruby: threads.map(&:join)
来源：http://cnz.snrcjt.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://cje.iojbl.cn

[O06] 使用进程池
来源：http://xmo.guannengcc.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sua.0kj1m.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://mkc.cdnleiting.top

JS:   // child_process / cluster 模块
来源：http://mzw.hywenlv.cn

TS:   // child_process / cluster 模块
来源：http://nsm.yuxming.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xpw.pycfn.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uzm.cqqwz.cn

Ruby: // fork 块
来源：http://gpb.tian-w.cn

C#:   Parallel.For
来源：http://bny.cucudq.cn

================================================================================
来源：http://vyu.sufxvd.cn

P. 常用工具函数
来源：http://uue.andypj.xyz

================================================================================
来源：http://qgn.shanyushiyangkeji.top

[P01] 生成 UUID
来源：http://vby.hnxiangtu.top

Py:   str(uuid.uuid4())
来源：http://xwy.chenzaomai.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wyc.zhengqikj.top

JS:   crypto.randomUUID()
来源：http://rqu.fengsongda.top

TS:   crypto.randomUUID()
来源：http://rtq.jinyuanbaomall.cn

Java: UUID.randomUUID().toString()
来源：http://xpf.ehwqpu.com

Go:   // 用 github.com/google/uuid
来源：http://pih.andypj.xyz

Ruby: SecureRandom.uuid
来源：http://xrd.cucudq.cn

C#:   Guid.NewGuid().ToString()
来源：http://rsx.tianlin.xyz

[P02] MD5 / SHA256 摘要
来源：http://boa.sweek.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ccs.daxiang520.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://boi.jinqigfzy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://szu.fengsongda.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ctu.zhengqikj.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://adb.jqgufenzy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://apm.shuidangran.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qfs.hnqzz.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vnm.smart0.xyz

[P03] 生成短随机字符串
来源：http://cia.ctjpmb.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://loj.daxiang520.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gkq.cucudq.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://owd.xuanzx.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://auh.jiagoushi.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tyh.yonumen.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rae.guannengcc.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://lvi.hammf.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zof.chenlongwang.top

[P04] 求长度
来源：http://rus.havefunace.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ccy.hongshengwenyu.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dpl.gogol.net.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zsg.jqgfzy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oxt.fengsongda.top

Java: list.size();  map.size();  s.length()
来源：http://auw.yj20258888.top

Go:   len(arr);  len(m)
来源：http://mqb.feifeiyinyue.top

Ruby: x.length;  x.size
来源：http://blx.svipenyu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xth.yuxming.cn

[P05] 判断两个对象内容是否相等
来源：http://uny.yj20258.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://mwh.yonumen.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rvz.cashguo.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://unr.sysykeji.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cpr.fengsongda.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xgd.kuanghao11.cn

Go:   reflect.DeepEqual(a, b)
来源：http://tav.redwolf501.top

Ruby: a == b
来源：http://bdk.fanxiaobao.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dvf.yueranfly.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://cjm.redwolf501.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zow.tanke756.top

PHP:  if (empty($x)) {}
来源：http://edn.vehdjk.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jau.nanxuanxn.top

TS:   if (x == null) {}
来源：http://wik.zhoulong.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://tlg.aibaodan.cn

Go:   if x == nil {}
来源：http://gnt.sweek.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ccz.ybcxt.top

C#:   if (x is null) {}
来源：http://oik.shanyushiyangkeji.top

[P07] 防抖与节流
来源：http://zge.jinyuanbaomall.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kre.ydzc1.top

PHP:  // 手写时间戳比较
来源：http://lin.cheryme.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://twf.jyoumei.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aai.cqqwz.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://avz.wangdashe.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kdm.jqgfzy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://yzx.shanyushiyangkeji.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://sec.yonumen.top

[P08] 处理浮点精度问题
来源：http://feh.zdqjudy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://whn.yfazqb.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://usd.xingfuxueyuan.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://aai.jinqigufen.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qrm.yj20258888.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://czf.yj20258.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zvg.yangfankeji.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vwr.yanxiufei.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://prk.jlsjyb.cn

================================================================================
来源：http://jqv.yueranfly.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ulr.mhx1999.top

================================================================================
来源：http://pkv.yuanzhike.top

[Q01] 创建表
来源：http://lmd.jinyuanbaomall.cn

CREATE TABLE users (
来源：http://pyy.zycfv.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zvy.haohaochexian.top

name VARCHAR(50) NOT NULL,
来源：http://shh.ybcxt.top

email VARCHAR(100) UNIQUE,
来源：http://iem.wangshuangyany.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pmp.hammf.cn

);
来源：http://fnb.cucudq.cn

[Q02] 创建带外键的表
来源：http://idm.ppjwa.cn

CREATE TABLE orders (
来源：http://npb.meibo888.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rep.smart0.xyz

user_id INT NOT NULL,
来源：http://wpq.daxiang520.top

amount DECIMAL(10, 2),
来源：http://ujm.vqdsnc.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tee.jiagoushi.top

);
来源：http://kre.tianlin.xyz

[Q03] 增加列
来源：http://fby.kuanghao11.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nua.shanyushiyangtech.top

[Q04] 修改列类型
来源：http://cbv.jlsjyb.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tap.tianlin.xyz

[Q05] 重命名列
来源：http://puk.snrcjt.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dos.aibaodan.cn

[Q06] 删除列
来源：http://wwh.hfpthk.cn

ALTER TABLE users DROP COLUMN age;
来源：http://rpr.chenlongwang.top

[Q07] 删除表
来源：http://jvg.tarul.cn

DROP TABLE IF EXISTS orders;
来源：http://xck.shanyushiyangkeji.top

[Q08] 创建普通索引
来源：http://ewo.xinyue.icu

CREATE INDEX idx_users_email ON users(email);
来源：http://kzd.guowangkeji.top

[Q09] 创建唯一索引
来源：http://tjb.snrcjt.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lyl.ybcxt.top

[Q10] 插入单行
来源：http://zks.ywan-chungtsiang.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jiz.316326.xyz

[Q11] 一次插入多行
来源：http://qoy.jqgufenzy.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://evh.chenzaomai.com

[Q12] 插入后取自增 ID
来源：http://kut.meibo888.top

INSERT INTO users (name) VALUES ('C');
来源：http://wae.zhixingplan.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mdn.tanke756.top

[Q13] 忽略重复插入
来源：http://zkk.zhiwuduotai.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gkj.xuanzx.com

[Q14] 存在则更新（upsert）
来源：http://hqs.zhiwuduotai.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kiq.vehdjk.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rvt.hesvh.cn

[Q15] 查询全部
来源：http://asy.hysaishi.cn

SELECT * FROM users;
来源：http://vge.gogol.net.cn

[Q16] 查询指定列
来源：http://hum.tarul.cn

SELECT id, name FROM users;
来源：http://ufb.tianlin.xyz

[Q17] 条件查询
来源：http://vtp.fzhhl.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dbq.sxryk.cn

[Q18] 模糊匹配
来源：http://fug.dianchejie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zzo.feifeiyinyue.top

[Q19] 范围查询
来源：http://hbd.cqqwz.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gkd.ybcxt.top

[Q20] IN 列表
来源：http://puo.chenlongwang.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://sdk.sufxvd.cn

[Q21] 空值判断
来源：http://ffg.shanyushiyangtech.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ooj.xuetiantiany.cn

[Q22] 排序
来源：http://mtg.nwbrower.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://icy.aibaodan.cn

[Q23] 分页
来源：http://vww.havefunace.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jxr.xylfe.cn

[Q24] 去重
来源：http://enh.dianchejie.cn

SELECT DISTINCT city FROM users;
来源：http://wgz.ydjk.org.cn

[Q25] 只取前 N 条
来源：http://ayz.jinqigufen.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gmk.hcnkem.com

[Q26] 计数
来源：http://ghb.guannengcc.top

SELECT COUNT(*) FROM users;
来源：http://erj.ydzc1.top

[Q27] 条件计数
来源：http://paq.zhiwuduotai.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gxq.jyoumei.cn

[Q28] 求和与平均
来源：http://kvh.sjlbkw.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zcv.aizwys.cn

[Q29] 最大最小值
来源：http://edp.smart0.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://szt.shanyushiyangtech.top

[Q30] 分组统计
来源：http://hvu.52xcode.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gcl.jyoumei.cn

[Q31] 分组后过滤
来源：http://kig.yuxming.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zkn.aibaodan.cn

[Q32] 分组拼接字符串
来源：http://mtu.tarul.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lna.aizwys.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hqg.ybcxt.top

[Q33] 多列分组
来源：http://vml.fengsongda.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://eba.nwbrower.top

[Q34] 每组取第一条
来源：http://jui.cheryme.top

SELECT * FROM (
来源：http://sxh.tian-w.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ear.shanyushiyangtech.top

) t WHERE rn = 1;
来源：http://uce.uphjek.com

[Q35] 内连接
来源：http://hkz.hesvh.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rvv.0kj1m.cn

[Q36] 左连接
来源：http://gfu.yj20258888.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ixw.quarkkingdee.top

[Q37] 右连接
来源：http://ieh.quarkkingdee.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rkb.hfpthk.cn

[Q38] 全外连接（PostgreSQL）
来源：http://gnn.hnqzz.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cxs.0kj1m.cn

[Q39] 自连接（查上下级）
来源：http://spp.yangfankeji.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://kds.nanxuanxn.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://syg.cqqwz.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://tbw.feifeiyinyue.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://txq.shangyingyoupin.top

[Q41] 多表连接
来源：http://pym.jqgfzy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ans.dashuyun.cn

JOIN users u ON u.id = o.user_id
来源：http://joz.hongshengwenyu.top

JOIN products p ON p.id = o.product_id;
来源：http://cxr.nwbrower.top

[Q42] 连接条件附加过滤
来源：http://kon.hywenlv.cn

SELECT u.name, o.amount FROM users u
来源：http://rxq.chenzaomai.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rqw.zdqjudy.top

[Q43] 标量子查询
来源：http://iwm.xinyue.icu

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://elh.zycfv.cn

[Q44] IN 子查询
来源：http://xhp.0kj1m.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mmq.zdqjudy.top

[Q45] EXISTS 判断存在
来源：http://wup.xuetiantiany.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qum.zycfv.cn

[Q46] NOT EXISTS 判断不存在
来源：http://tdc.xinyue.icu

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bkq.hnqzz.top

[Q47] 与平均值比较
来源：http://dyq.zycfv.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://sqp.pengpengdd.cyou

[Q48] CTE 公用表表达式
来源：http://zsx.ctjpmb.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ziw.bjfxy.top

SELECT * FROM t WHERE c > 5;
来源：http://vdf.yuxming.cn

[Q49] 更新单行
来源：http://ald.aibaodan.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rqi.jinqigufen.top

[Q50] 批量更新
来源：http://czl.zdqjudy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hqo.feifeiyinyue.top

[Q51] 用子查询更新
来源：http://jlf.zdqjudy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xrq.ywan-chungtsiang.top

[Q52] 删除指定行
来源：http://ron.yj20258.top

DELETE FROM users WHERE id = 10;
来源：http://joc.jqgfzy.top

[Q53] 按条件删除
来源：http://dvn.shzxlz.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rom.bbcook.cn

[Q54] 清空表
来源：http://pjj.shzxlz.cn

TRUNCATE TABLE logs;
来源：http://fxb.wangshuangyany.cn

[Q55] 排名（并列占位）
来源：http://xel.nanxinkj.top


<!-- 参考信息 -->
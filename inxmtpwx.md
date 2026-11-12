代发 wailian999

[N09] 栈与队列
来源：http://wrp.dashuyun.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tmr.pycfn.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kci.cucudq.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://owl.vehdjk.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baq.yangfankeji.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ois.yuanzhike.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mlc.snrcjt.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ikr.yangfankeji.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xql.ywan-chungtsiang.top

[N10] 链表节点定义
来源：http://trk.shanyushiyangtech.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://opf.yangfankeji.com

PHP:  class Node { public $v; public $next = null; }
来源：http://bgy.hfpthk.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ygz.shangyingyoupin.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zel.aibaodan.cn

Java: class Node { int v; Node next; }
来源：http://gvl.sxryk.cn

Go:   type Node struct { V int; Next *Node }
来源：http://yvg.c1oappe.top

Ruby: Node = Struct.new(:v, :next)
来源：http://jmh.hysaishi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://eze.birdmap.top

[N11] 二叉树中序遍历
来源：http://fre.sufxvd.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ejw.hongshengwenyu.top

PHP:  // 手写递归函数
来源：http://agp.zhongyouzk.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sgw.cqqwz.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nwq.zhiwuduotai.top

Java: // 手写递归
来源：http://rmg.hfpthk.cn

Go:   // 手写递归
来源：http://dpe.jinqigufen.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ezd.hesvh.cn

C#:   // 手写递归
来源：http://vpj.ydzc1.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ulu.shuidangran.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qmp.cashguo.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rqq.cdnleiting.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://esc.xinyue.icu

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nie.shanyushiyangkeji.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tkk.yanxiufei.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wqw.yfazqb.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mbp.hongshengwenyu.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ara.sxryk.cn

================================================================================
来源：http://zhc.tanke756.top

O. 并发与异步
来源：http://ffz.shangyingyoupin.top

================================================================================
来源：http://tmz.haohaochexian.top

[O01] 启动一个线程
来源：http://vxb.xuetiantiany.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cwn.wangdashe.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xeo.fengsongda.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yfv.kuanghao11.cn

TS:   // 同 JS
来源：http://cup.chenlongwang.top

Java: new Thread(() -> f()).start()
来源：http://lva.jinqigfzy.top

Go:   go f()
来源：http://oeq.shanyushiyangtech.top

Ruby: Thread.new { f }
来源：http://hvi.jinqigufen.top

C#:   Task.Run(() => F());
来源：http://kaq.haohaochexian.top

[O02] 使用线程池
来源：http://egv.guowangkeji.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cdo.aizwys.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tuc.vehdjk.com

JS:   // worker_threads 线程池
来源：http://tvi.nanxuanxn.top

TS:   // worker_threads 线程池
来源：http://ust.jiagoushi.top

Java: Executors.newFixedThreadPool(4)
来源：http://vbv.iojbl.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bmj.gotoacloud.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cze.yongpay.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://glh.cdnleiting.top

[O03] 加锁保护共享数据
来源：http://pwx.jqgufenzy.top

Py:   with lock: shared += 1
来源：http://iby.sysykeji.top

PHP:  // 用 flock() 做文件锁
来源：http://xop.gogol.net.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gda.xziqi.cn

TS:   // 同 JS
来源：http://moy.tianlin.xyz

Java: synchronized (this) { shared++; }
来源：http://lep.yongpay.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hjj.snrcjt.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://qvq.xylfe.cn

C#:   lock (gate) { shared++; }
来源：http://qrf.sxryk.cn

[O04] 定义异步函数并等待
来源：http://htn.shangyingyoupin.top

Py:   async def f():⏎    await g()
来源：http://mvp.pengpengdd.cyou

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vef.zhoulong.xyz

JS:   async function f() { await g(); }
来源：http://rrt.feifeiyinyue.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://poe.ctjpmb.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://btv.ydjk.org.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dvy.zhiwuduotai.top

Ruby: # 用 Fiber 或 async gem
来源：http://vyt.shanyushiyangkeji.top

C#:   async Task F() { await G(); }
来源：http://hrg.hcnkem.com

[O05] 并发执行并等待全部完成
来源：http://wkw.tian-w.cn

Py:   asyncio.gather(*tasks)
来源：http://lft.kuanghao11.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mzi.uphjek.com

JS:   await Promise.all(tasks)
来源：http://gfm.ivvv.top

TS:   await Promise.all(tasks)
来源：http://hwg.hfpthk.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dsd.yongpay.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gta.nwbrower.top

Ruby: threads.map(&:join)
来源：http://ylf.sxryk.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qgk.uphjek.com

[O06] 使用进程池
来源：http://qbz.guannengcc.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jtt.zhijiandao.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://jgs.yonumen.top

JS:   // child_process / cluster 模块
来源：http://mno.vehdjk.com

TS:   // child_process / cluster 模块
来源：http://cxy.xylfe.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qnf.zdqjudy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cky.aizwys.cn

Ruby: // fork 块
来源：http://ghi.zhiwuduotai.top

C#:   Parallel.For
来源：http://xqg.ppjwa.cn

================================================================================
来源：http://gsz.ywan-chungtsiang.top

P. 常用工具函数
来源：http://kgm.wangshuangyany.cn

================================================================================
来源：http://jzx.chenlongwang.top

[P01] 生成 UUID
来源：http://xnh.shangyingyoupin.top

Py:   str(uuid.uuid4())
来源：http://bwq.yuanzhike.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ofi.bbcook.cn

JS:   crypto.randomUUID()
来源：http://abh.gotoacloud.top

TS:   crypto.randomUUID()
来源：http://zfl.pengpengdd.cyou

Java: UUID.randomUUID().toString()
来源：http://hur.wangshuangyany.cn

Go:   // 用 github.com/google/uuid
来源：http://yse.vqdsnc.cn

Ruby: SecureRandom.uuid
来源：http://nuh.dashuyun.cn

C#:   Guid.NewGuid().ToString()
来源：http://rnu.nanxinkj.top

[P02] MD5 / SHA256 摘要
来源：http://xhf.yuanzhike.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jep.chenzaomai.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://lud.ydjk.org.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://koc.andypj.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lte.hesvh.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://drr.hnqzz.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hae.jqgfzy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ttb.sweek.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zct.xuanzx.com

[P03] 生成短随机字符串
来源：http://mna.yueranfly.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mpa.dianchejie.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nhe.tanke756.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jxa.ivvv.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://czw.xinyue.icu

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ihg.epnwcf.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vlf.redwolf501.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://agu.zhengqikj.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cwy.zhijiandao.cn

[P04] 求长度
来源：http://xzt.wangshuangyany.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ekj.sjlbkw.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://owm.tianlin.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://avx.yj202588.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yhr.yvedp.cn

Java: list.size();  map.size();  s.length()
来源：http://puz.daria6918.cn

Go:   len(arr);  len(m)
来源：http://ilg.andypj.xyz

Ruby: x.length;  x.size
来源：http://dkr.chenjidiqi.icu

C#:   list.Count;  dict.Count;  s.Length
来源：http://rpa.zycfv.cn

[P05] 判断两个对象内容是否相等
来源：http://qag.sweek.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://adv.ydzc1.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bbx.tanke756.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://brm.xingfuxueyuan.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qfq.hywenlv.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ypr.shanyushiyangtech.top

Go:   reflect.DeepEqual(a, b)
来源：http://owt.yj20258.top

Ruby: a == b
来源：http://frs.0kj1m.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lxz.hysaishi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://emd.smart0.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sjr.uphjek.com

PHP:  if (empty($x)) {}
来源：http://dvm.wangdashe.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://znw.hnxiangtu.top

TS:   if (x == null) {}
来源：http://iae.yonumen.top

Java: if (x == null || x.isEmpty()) {}
来源：http://fxq.316326.xyz

Go:   if x == nil {}
来源：http://byq.zhongyouzk.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dwl.birdmap.top

C#:   if (x is null) {}
来源：http://cwl.ctjpmb.com

[P07] 防抖与节流
来源：http://njo.9152youxi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://geb.zhongyouzk.top

PHP:  // 手写时间戳比较
来源：http://kfy.yj20258888.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fnt.pengpengdd.cyou

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cfi.jinghuilouyu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gef.hammf.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gwd.sufxvd.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://yqe.jiagoushi.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xnk.iojbl.cn

[P08] 处理浮点精度问题
来源：http://hdz.sysykeji.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://avo.yuxming.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://tvv.sysykeji.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qtr.hongshengwenyu.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kdt.yuxming.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vhs.aizwys.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://eiy.wangshuangyany.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mdo.cashguo.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zqv.bjfxy.top

================================================================================
来源：http://kma.aibaodan.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qnt.chenjidiqi.icu

================================================================================
来源：http://shj.hnxiangtu.top

[Q01] 创建表
来源：http://ort.ydjk.org.cn

CREATE TABLE users (
来源：http://ixs.wangshuangyany.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zmq.tarul.cn

name VARCHAR(50) NOT NULL,
来源：http://bcd.smart0.xyz

email VARCHAR(100) UNIQUE,
来源：http://zva.kuanghao11.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gce.gogol.net.cn

);
来源：http://fze.pengpengdd.cyou

[Q02] 创建带外键的表
来源：http://skz.aibaodan.cn

CREATE TABLE orders (
来源：http://sjm.yvedp.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jot.hnqzz.top

user_id INT NOT NULL,
来源：http://mgy.hywenlv.cn

amount DECIMAL(10, 2),
来源：http://fyw.smart0.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gno.daria6918.cn

);
来源：http://usd.svipenyu.cn

[Q03] 增加列
来源：http://fsy.yvedp.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bgg.0kj1m.cn

[Q04] 修改列类型
来源：http://lsa.dashuyun.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yiu.jyoumei.cn

[Q05] 重命名列
来源：http://pss.yj202588.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pef.nanxinkj.top

[Q06] 删除列
来源：http://xkd.yongpay.top

ALTER TABLE users DROP COLUMN age;
来源：http://wbe.yonumen.top

[Q07] 删除表
来源：http://hhp.cheryme.top

DROP TABLE IF EXISTS orders;
来源：http://tsy.ehwqpu.com

[Q08] 创建普通索引
来源：http://lgn.tian-w.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://aba.zdbjq.cn

[Q09] 创建唯一索引
来源：http://uum.zhixingplan.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://sse.xinyue.icu

[Q10] 插入单行
来源：http://ula.gogol.net.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mwy.tanke756.top

[Q11] 一次插入多行
来源：http://qyf.nanxinkj.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qtm.jinyuanbaomall.cn

[Q12] 插入后取自增 ID
来源：http://jmw.zhongyouzk.top

INSERT INTO users (name) VALUES ('C');
来源：http://mqf.shanyushiyangkeji.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dij.yongpay.top

[Q13] 忽略重复插入
来源：http://rcz.svipenyu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qus.jinqigfzy.top

[Q14] 存在则更新（upsert）
来源：http://inv.yj202588.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://huh.pycfn.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dft.uphjek.com

[Q15] 查询全部
来源：http://qjb.fzhhl.top

SELECT * FROM users;
来源：http://rbl.yj202588.top

[Q16] 查询指定列
来源：http://qyd.zhoulong.xyz

SELECT id, name FROM users;
来源：http://asb.yfazqb.com

[Q17] 条件查询
来源：http://ypv.epnwcf.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jjx.tianlin.xyz

[Q18] 模糊匹配
来源：http://gmy.jqgfzy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zmx.316326.xyz

[Q19] 范围查询
来源：http://mec.feifeiyinyue.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://sxn.cqqwz.cn

[Q20] IN 列表
来源：http://wvj.redwolf501.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zml.jyoumei.cn

[Q21] 空值判断
来源：http://pen.dashuyun.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://rlw.zdbjq.cn

[Q22] 排序
来源：http://qxu.zhixingplan.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://glw.yvedp.cn

[Q23] 分页
来源：http://bjs.jiagoushi.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://inj.shzxlz.cn

[Q24] 去重
来源：http://bjw.shzxlz.cn

SELECT DISTINCT city FROM users;
来源：http://atx.shanyushiyangkeji.top

[Q25] 只取前 N 条
来源：http://jvh.yanxiufei.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pxp.gaohongyu789.top

[Q26] 计数
来源：http://dtb.hysaishi.cn

SELECT COUNT(*) FROM users;
来源：http://gcm.hnqzz.top

[Q27] 条件计数
来源：http://wmz.ydzc1.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bch.wangshuangyany.cn

[Q28] 求和与平均
来源：http://rbe.sweek.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ump.xziqi.cn

[Q29] 最大最小值
来源：http://pmp.yonumen.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://zdf.iojbl.cn

[Q30] 分组统计
来源：http://ele.cdnleiting.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://kxk.epnwcf.com

[Q31] 分组后过滤
来源：http://vsn.ehwqpu.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jkb.chenjidiqi.icu

[Q32] 分组拼接字符串
来源：http://voj.cheryme.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mpg.hcnkem.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kcr.gotoacloud.top

[Q33] 多列分组
来源：http://ffx.vehdjk.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lyi.bbcook.cn

[Q34] 每组取第一条
来源：http://ain.guowangkeji.top

SELECT * FROM (
来源：http://tyy.ydzc1.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ksw.aizwys.cn

) t WHERE rn = 1;
来源：http://ldq.52xcode.cn

[Q35] 内连接
来源：http://dfw.yj202588.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://okh.zhixingplan.top

[Q36] 左连接
来源：http://pcv.yuanzhike.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qlg.fehbvm.com

[Q37] 右连接
来源：http://cax.cdnleiting.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qyh.cucudq.cn

[Q38] 全外连接（PostgreSQL）
来源：http://brs.cashguo.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wth.mhx1999.top

[Q39] 自连接（查上下级）
来源：http://tpz.zdqjudy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://iax.nwbrower.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jne.yonumen.top

[Q40] 交叉连接（笛卡尔积）
来源：http://wjv.zhaomingkeji.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qgo.ywan-chungtsiang.top

[Q41] 多表连接
来源：http://dbo.hnxiangtu.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://qjn.dashuyun.cn

JOIN users u ON u.id = o.user_id
来源：http://cap.bbcook.cn

JOIN products p ON p.id = o.product_id;
来源：http://tez.ydzc1.top

[Q42] 连接条件附加过滤
来源：http://efv.gotoacloud.top

SELECT u.name, o.amount FROM users u
来源：http://cif.fzhhl.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gzq.wangshuangyany.cn

[Q43] 标量子查询
来源：http://byx.jinghuilouyu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vsy.xuetiantiany.cn

[Q44] IN 子查询
来源：http://qlk.wangdashe.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yjx.sxryk.cn

[Q45] EXISTS 判断存在
来源：http://crx.fktsv.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fkn.hcnkem.com

[Q46] NOT EXISTS 判断不存在
来源：http://zvd.hywenlv.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dmn.tian-w.cn

[Q47] 与平均值比较
来源：http://sjk.fehbvm.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://aim.52xcode.cn

[Q48] CTE 公用表表达式
来源：http://ksp.wangshuangyany.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hmy.tian-w.cn

SELECT * FROM t WHERE c > 5;
来源：http://hpw.sufxvd.cn

[Q49] 更新单行
来源：http://scv.vqdsnc.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dzs.sysykeji.top

[Q50] 批量更新
来源：http://tbo.jlsjyb.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cpi.nwbrower.top

[Q51] 用子查询更新
来源：http://zxr.chenlongwang.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://unq.c1oappe.top

[Q52] 删除指定行
来源：http://wij.tian-w.cn

DELETE FROM users WHERE id = 10;
来源：http://mef.jinqigfzy.top

[Q53] 按条件删除
来源：http://iba.yj202588.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://flv.c1oappe.top

[Q54] 清空表
来源：http://fbp.cheryme.top

TRUNCATE TABLE logs;
来源：http://kmj.shangyingyoupin.top

[Q55] 排名（并列占位）
来源：http://joa.jyoumei.cn


<!-- 参考信息 -->
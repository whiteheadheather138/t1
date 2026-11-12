代发 wailian999

[N09] 栈与队列
来源：http://wcf.xuetiantiany.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tan.hywenlv.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gvo.fktsv.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mxh.ivvv.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vvw.hnxiangtu.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fdd.jianghu66.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xxu.tarul.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kik.gogol.net.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ltf.hesvh.cn

[N10] 链表节点定义
来源：http://jxo.jinghuilouyu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xym.xziqi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://vtk.c1oappe.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nca.zycfv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gwa.gaohongyu789.top

Java: class Node { int v; Node next; }
来源：http://kxn.gaohongyu789.top

Go:   type Node struct { V int; Next *Node }
来源：http://dwq.jqgfzy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://cyx.hnqzz.top

C#:   class Node { public int V; public Node? Next; }
来源：http://mmq.ybcxt.top

[N11] 二叉树中序遍历
来源：http://tcg.hongshengwenyu.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pox.yvedp.cn

PHP:  // 手写递归函数
来源：http://xhj.yanxiufei.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yea.0kj1m.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cjb.aibaodan.cn

Java: // 手写递归
来源：http://rfm.shanyushiyangkeji.top

Go:   // 手写递归
来源：http://aiy.hysaishi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://frf.fktsv.cn

C#:   // 手写递归
来源：http://pok.cdnleiting.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://oqf.bbcook.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://azq.aizwys.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tbb.tarul.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gli.fengsongda.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://awa.shanyushiyangtech.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://thu.aibaodan.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ewt.cashguo.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://puy.52xcode.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vxa.birdmap.top

================================================================================
来源：http://tlw.chenlongwang.top

O. 并发与异步
来源：http://amd.sxryk.cn

================================================================================
来源：http://wkk.hysaishi.cn

[O01] 启动一个线程
来源：http://kxm.daria6918.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://twz.wangshuangyany.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nvz.jyoumei.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pdq.yj20258.top

TS:   // 同 JS
来源：http://nrc.havefunace.top

Java: new Thread(() -> f()).start()
来源：http://ija.hysaishi.cn

Go:   go f()
来源：http://vvk.havefunace.top

Ruby: Thread.new { f }
来源：http://wtz.gogol.net.cn

C#:   Task.Run(() => F());
来源：http://jcc.chenzaomai.com

[O02] 使用线程池
来源：http://mtj.jyoumei.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://old.jinqigufen.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sdd.cucudq.cn

JS:   // worker_threads 线程池
来源：http://hhc.chenjidiqi.icu

TS:   // worker_threads 线程池
来源：http://twy.dianchejie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://nbz.zycfv.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zja.wangshuangyany.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pwo.chenzaomai.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qkz.xinyue.icu

[O03] 加锁保护共享数据
来源：http://bbv.ydzc1.top

Py:   with lock: shared += 1
来源：http://kco.meibo888.top

PHP:  // 用 flock() 做文件锁
来源：http://urw.aibaodan.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dff.cashguo.top

TS:   // 同 JS
来源：http://moe.vehdjk.com

Java: synchronized (this) { shared++; }
来源：http://jsd.kuanghao11.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xog.yvedp.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://neh.zhixingplan.top

C#:   lock (gate) { shared++; }
来源：http://qro.zhongyouzk.top

[O04] 定义异步函数并等待
来源：http://bsf.sweek.top

Py:   async def f():⏎    await g()
来源：http://qfc.fktsv.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tvw.wangshuangyany.cn

JS:   async function f() { await g(); }
来源：http://dsm.zhongyouzk.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://pnz.52xcode.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pse.jlsjyb.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bix.kuanghao11.cn

Ruby: # 用 Fiber 或 async gem
来源：http://oaf.bbcook.cn

C#:   async Task F() { await G(); }
来源：http://lcg.sxryk.cn

[O05] 并发执行并等待全部完成
来源：http://zca.snrcjt.cn

Py:   asyncio.gather(*tasks)
来源：http://gfk.jyoumei.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://byq.bbcook.cn

JS:   await Promise.all(tasks)
来源：http://uqi.andypj.xyz

TS:   await Promise.all(tasks)
来源：http://wip.cucudq.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bjf.shuidangran.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gyf.jinyuanbaomall.cn

Ruby: threads.map(&:join)
来源：http://zde.aibaodan.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://gtp.pycfn.com

[O06] 使用进程池
来源：http://gyi.yonumen.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hbv.chenjidiqi.icu

PHP:  // pcntl_fork 或多进程队列
来源：http://man.dashuyun.cn

JS:   // child_process / cluster 模块
来源：http://zfv.wangdashe.top

TS:   // child_process / cluster 模块
来源：http://kry.iojbl.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://enf.xuetiantiany.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kgb.chenjidiqi.icu

Ruby: // fork 块
来源：http://vzv.cheryme.top

C#:   Parallel.For
来源：http://zqh.gotoacloud.top

================================================================================
来源：http://nyf.ybcxt.top

P. 常用工具函数
来源：http://iac.sweek.top

================================================================================
来源：http://xuj.sxryk.cn

[P01] 生成 UUID
来源：http://myq.xingfuxueyuan.xyz

Py:   str(uuid.uuid4())
来源：http://ohb.jinghuilouyu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dcf.xingfuxueyuan.xyz

JS:   crypto.randomUUID()
来源：http://wpk.quarkkingdee.top

TS:   crypto.randomUUID()
来源：http://qrj.xingfuxueyuan.xyz

Java: UUID.randomUUID().toString()
来源：http://gyj.yj202588.top

Go:   // 用 github.com/google/uuid
来源：http://cxj.hnxiangtu.top

Ruby: SecureRandom.uuid
来源：http://nen.quarkkingdee.top

C#:   Guid.NewGuid().ToString()
来源：http://jgj.redwolf501.top

[P02] MD5 / SHA256 摘要
来源：http://tkb.52xcode.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://unf.yuxming.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://jiu.mhx1999.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bwr.jlsjyb.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hml.gzhubu.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zjm.zycfv.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vvu.hfpthk.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://eoh.wangshuangyany.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ges.gotoacloud.top

[P03] 生成短随机字符串
来源：http://pkd.vqdsnc.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://llx.sysykeji.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dhz.hcnkem.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cka.dashuyun.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nnw.fzhhl.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dvd.snrcjt.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://utt.bbcook.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ojy.hongshengwenyu.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yub.dianchejie.cn

[P04] 求长度
来源：http://gpd.cashguo.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cao.ctjpmb.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fns.epnwcf.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iic.yanxiufei.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nww.xuanzx.com

Java: list.size();  map.size();  s.length()
来源：http://djx.xuanzx.com

Go:   len(arr);  len(m)
来源：http://crt.jiagoushi.top

Ruby: x.length;  x.size
来源：http://xaz.gaohongyu789.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://rhj.guowangkeji.top

[P05] 判断两个对象内容是否相等
来源：http://ljf.xuetiantiany.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://fmu.zdbjq.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qou.jinghuilouyu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qhg.ybcxt.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nwh.gaohongyu789.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://euz.cucudq.cn

Go:   reflect.DeepEqual(a, b)
来源：http://yor.cdnleiting.top

Ruby: a == b
来源：http://vrr.aizwys.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://efu.jinqigfzy.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qzd.cheryme.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fks.cheryme.top

PHP:  if (empty($x)) {}
来源：http://xxe.vqdsnc.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://akj.hesvh.cn

TS:   if (x == null) {}
来源：http://gxf.fktsv.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://xie.haohaochexian.top

Go:   if x == nil {}
来源：http://yqg.aibaodan.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zsj.feifeiyinyue.top

C#:   if (x is null) {}
来源：http://swo.zhixingplan.top

[P07] 防抖与节流
来源：http://teg.vqdsnc.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hbo.wangshuangyany.cn

PHP:  // 手写时间戳比较
来源：http://opd.zdqjudy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ysa.bbcook.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://imm.gogol.net.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wwd.xuanzx.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gjv.zdbjq.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://jde.52xcode.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lgb.tarul.cn

[P08] 处理浮点精度问题
来源：http://yqm.hfpthk.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://chz.dashuyun.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wax.316326.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vgx.gzhubu.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rta.ybcxt.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://eyd.zhijiandao.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xam.zhijiandao.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hkc.tianlin.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xhi.hfpthk.cn

================================================================================
来源：http://ebj.mhx1999.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zyf.xingfuxueyuan.xyz

================================================================================
来源：http://hkd.mhx1999.top

[Q01] 创建表
来源：http://zxu.dianchejie.cn

CREATE TABLE users (
来源：http://nsp.sjlbkw.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fgb.ehwqpu.com

name VARCHAR(50) NOT NULL,
来源：http://ucp.daria6918.cn

email VARCHAR(100) UNIQUE,
来源：http://dvi.shanyushiyangtech.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://djw.sysykeji.top

);
来源：http://uki.zycfv.cn

[Q02] 创建带外键的表
来源：http://tmz.cashguo.top

CREATE TABLE orders (
来源：http://kch.yuanzhike.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vuc.sxryk.cn

user_id INT NOT NULL,
来源：http://viw.zycfv.cn

amount DECIMAL(10, 2),
来源：http://mtw.fanxiaobao.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://uza.c1oappe.top

);
来源：http://wdk.tanke756.top

[Q03] 增加列
来源：http://kof.quarkkingdee.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xfa.ehwqpu.com

[Q04] 修改列类型
来源：http://snf.ydjk.org.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://nyq.zhongyouzk.top

[Q05] 重命名列
来源：http://pnq.nanxinkj.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jky.pengpengdd.cyou

[Q06] 删除列
来源：http://pry.cucudq.cn

ALTER TABLE users DROP COLUMN age;
来源：http://uqw.pycfn.com

[Q07] 删除表
来源：http://oqe.ybcxt.top

DROP TABLE IF EXISTS orders;
来源：http://lji.yongpay.top

[Q08] 创建普通索引
来源：http://prn.birdmap.top

CREATE INDEX idx_users_email ON users(email);
来源：http://qau.cqqwz.cn

[Q09] 创建唯一索引
来源：http://zcy.cdnleiting.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zhr.snrcjt.cn

[Q10] 插入单行
来源：http://kas.cqqwz.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://bnf.yueranfly.top

[Q11] 一次插入多行
来源：http://fqc.xuanzx.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dox.fzhhl.top

[Q12] 插入后取自增 ID
来源：http://qcn.gaohongyu789.top

INSERT INTO users (name) VALUES ('C');
来源：http://jci.shanyushiyangkeji.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qcb.gogol.net.cn

[Q13] 忽略重复插入
来源：http://hzb.daria6918.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ebx.ybcxt.top

[Q14] 存在则更新（upsert）
来源：http://dde.chenlongwang.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ehp.pycfn.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://iad.bjfxy.top

[Q15] 查询全部
来源：http://ubp.tianlin.xyz

SELECT * FROM users;
来源：http://evn.fzhhl.top

[Q16] 查询指定列
来源：http://nbm.yueranfly.top

SELECT id, name FROM users;
来源：http://xwv.xinyue.icu

[Q17] 条件查询
来源：http://jil.jinqigfzy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fex.dianchejie.cn

[Q18] 模糊匹配
来源：http://jso.yongpay.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ttn.jiagoushi.top

[Q19] 范围查询
来源：http://nmr.bjfxy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tli.snrcjt.cn

[Q20] IN 列表
来源：http://asu.sysykeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nsi.jianghu66.top

[Q21] 空值判断
来源：http://mnz.guannengcc.top

SELECT * FROM users WHERE email IS NULL;
来源：http://nqc.uphjek.com

[Q22] 排序
来源：http://oer.yanxiufei.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ylq.zhengqikj.top

[Q23] 分页
来源：http://ane.birdmap.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wyu.shzxlz.cn

[Q24] 去重
来源：http://thq.quarkkingdee.top

SELECT DISTINCT city FROM users;
来源：http://cxb.dashuyun.cn

[Q25] 只取前 N 条
来源：http://qol.cheryme.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vrh.hongshengwenyu.top

[Q26] 计数
来源：http://epc.ywan-chungtsiang.top

SELECT COUNT(*) FROM users;
来源：http://bnq.gzhubu.top

[Q27] 条件计数
来源：http://dam.xuanzx.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wbm.hfpthk.cn

[Q28] 求和与平均
来源：http://xoi.feifeiyinyue.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://frz.ydjk.org.cn

[Q29] 最大最小值
来源：http://gpa.pengpengdd.cyou

SELECT MAX(age), MIN(age) FROM users;
来源：http://bau.sysykeji.top

[Q30] 分组统计
来源：http://zth.ppjwa.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dfv.yuxming.cn

[Q31] 分组后过滤
来源：http://viu.chenzaomai.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hbv.xingfuxueyuan.xyz

[Q32] 分组拼接字符串
来源：http://iyd.cqqwz.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dvd.jinyuanbaomall.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ozw.iojbl.cn

[Q33] 多列分组
来源：http://sls.havefunace.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rrc.gogol.net.cn

[Q34] 每组取第一条
来源：http://agb.nanxuanxn.top

SELECT * FROM (
来源：http://blr.guowangkeji.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bod.zhiwuduotai.top

) t WHERE rn = 1;
来源：http://gxe.nanxuanxn.top

[Q35] 内连接
来源：http://esj.hnxiangtu.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ikp.tianlin.xyz

[Q36] 左连接
来源：http://yws.9152youxi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wgi.tianlin.xyz

[Q37] 右连接
来源：http://aak.jqgufenzy.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uyh.sxryk.cn

[Q38] 全外连接（PostgreSQL）
来源：http://wwj.aibaodan.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://twy.ybcxt.top

[Q39] 自连接（查上下级）
来源：http://jui.xinyue.icu

SELECT e.name, m.name AS manager FROM employees e
来源：http://roo.chenzaomai.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qpw.sufxvd.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://yjm.daxiang520.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tvv.yanxiufei.cn

[Q41] 多表连接
来源：http://uoo.zdqjudy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://jvw.yj20258888.top

JOIN users u ON u.id = o.user_id
来源：http://bsk.guowangkeji.top

JOIN products p ON p.id = o.product_id;
来源：http://aad.jqgufenzy.top

[Q42] 连接条件附加过滤
来源：http://uch.feifeiyinyue.top

SELECT u.name, o.amount FROM users u
来源：http://lmr.zhengqikj.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xzg.9152youxi.cn

[Q43] 标量子查询
来源：http://ccb.jinyuanbaomall.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dgn.chenlongwang.top

[Q44] IN 子查询
来源：http://ddu.xylfe.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gfa.bjfxy.top

[Q45] EXISTS 判断存在
来源：http://tdm.yangfankeji.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jxq.nanxinkj.top

[Q46] NOT EXISTS 判断不存在
来源：http://dbc.hcnkem.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xho.zdbjq.cn

[Q47] 与平均值比较
来源：http://sdf.xuanzx.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vhv.shanyushiyangtech.top

[Q48] CTE 公用表表达式
来源：http://rsg.dashuyun.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gaw.kuanghao11.cn

SELECT * FROM t WHERE c > 5;
来源：http://xma.shanyushiyangtech.top

[Q49] 更新单行
来源：http://acj.feifeiyinyue.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://own.yuanzhike.top

[Q50] 批量更新
来源：http://ugb.ivvv.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://eih.tanke756.top

[Q51] 用子查询更新
来源：http://hie.sxryk.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://uer.zdbjq.cn

[Q52] 删除指定行
来源：http://gff.fengsongda.top

DELETE FROM users WHERE id = 10;
来源：http://yzo.sweek.top

[Q53] 按条件删除
来源：http://mlw.jqgfzy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jnn.yj20258888.top

[Q54] 清空表
来源：http://mjk.jinqigfzy.top

TRUNCATE TABLE logs;
来源：http://rzq.smart0.xyz

[Q55] 排名（并列占位）
来源：http://veq.ybcxt.top


<!-- 参考信息 -->
代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://umw.aibaodan.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tgd.yongpay.top

Java: class Node { int v; Node next; }
来源：http://fsw.tanke756.top

Go:   type Node struct { V int; Next *Node }
来源：http://hoo.yj20258.top

Ruby: Node = Struct.new(:v, :next)
来源：http://mia.shanyushiyangtech.top

C#:   class Node { public int V; public Node? Next; }
来源：http://lfv.ydzc1.top

[N11] 二叉树中序遍历
来源：http://qdi.aibaodan.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mtq.zhengqikj.top

PHP:  // 手写递归函数
来源：http://kju.sweek.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wps.zdqjudy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cqw.shanyushiyangkeji.top

Java: // 手写递归
来源：http://ske.gogol.net.cn

Go:   // 手写递归
来源：http://rwb.zycfv.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gqv.yfazqb.com

C#:   // 手写递归
来源：http://nwm.316326.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cto.andypj.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jqw.hnxiangtu.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jmx.0kj1m.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zmt.fehbvm.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vyt.smart0.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pma.tarul.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://upz.fktsv.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://obf.jiagoushi.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ecr.zhongyouzk.top

================================================================================
来源：http://pas.ivvv.top

O. 并发与异步
来源：http://iua.zhijiandao.cn

================================================================================
来源：http://vuv.epnwcf.com

[O01] 启动一个线程
来源：http://yob.hnxiangtu.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tdn.zdbjq.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tji.cashguo.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://aod.dianchejie.cn

TS:   // 同 JS
来源：http://rqg.gogol.net.cn

Java: new Thread(() -> f()).start()
来源：http://url.kuanghao11.cn

Go:   go f()
来源：http://bxo.jyoumei.cn

Ruby: Thread.new { f }
来源：http://tdw.uphjek.com

C#:   Task.Run(() => F());
来源：http://lko.tianlin.xyz

[O02] 使用线程池
来源：http://miv.9152youxi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wck.bjfxy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tvw.shuidangran.top

JS:   // worker_threads 线程池
来源：http://qof.hfpthk.cn

TS:   // worker_threads 线程池
来源：http://sab.fanxiaobao.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://jzb.hysaishi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vua.tianlin.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://eep.52xcode.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pqi.hfpthk.cn

[O03] 加锁保护共享数据
来源：http://hlu.quarkkingdee.top

Py:   with lock: shared += 1
来源：http://krw.guannengcc.top

PHP:  // 用 flock() 做文件锁
来源：http://jhd.ivvv.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zfx.andypj.xyz

TS:   // 同 JS
来源：http://mgz.redwolf501.top

Java: synchronized (this) { shared++; }
来源：http://cwq.hcnkem.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qrt.yvedp.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://cbu.yanxiufei.cn

C#:   lock (gate) { shared++; }
来源：http://gzg.jianghu66.top

[O04] 定义异步函数并等待
来源：http://iey.cqqwz.cn

Py:   async def f():⏎    await g()
来源：http://yjv.jinyuanbaomall.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fvq.yueranfly.top

JS:   async function f() { await g(); }
来源：http://kim.yj202588.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ecw.ybcxt.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bhf.shzxlz.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cik.xingfuxueyuan.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://wit.haohaochexian.top

C#:   async Task F() { await G(); }
来源：http://stj.ctjpmb.com

[O05] 并发执行并等待全部完成
来源：http://fqp.sysykeji.top

Py:   asyncio.gather(*tasks)
来源：http://dub.fengsongda.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ysh.chenjidiqi.icu

JS:   await Promise.all(tasks)
来源：http://zxa.shangyingyoupin.top

TS:   await Promise.all(tasks)
来源：http://tex.uphjek.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rif.pengpengdd.cyou

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://eyx.zhengqikj.top

Ruby: threads.map(&:join)
来源：http://nao.zhixingplan.top

C#:   await Task.WhenAll(t1, t2)
来源：http://dcd.xylfe.cn

[O06] 使用进程池
来源：http://yiz.yj20258.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jtx.nanxuanxn.top

PHP:  // pcntl_fork 或多进程队列
来源：http://vxc.gaohongyu789.top

JS:   // child_process / cluster 模块
来源：http://roh.yfazqb.com

TS:   // child_process / cluster 模块
来源：http://vno.snrcjt.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ytw.sxryk.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ehn.xuanzx.com

Ruby: // fork 块
来源：http://ksk.sysykeji.top

C#:   Parallel.For
来源：http://twd.yanxiufei.cn

================================================================================
来源：http://hqf.chenzaomai.com

P. 常用工具函数
来源：http://vyu.svipenyu.cn

================================================================================
来源：http://kxz.cashguo.top

[P01] 生成 UUID
来源：http://wum.bjfxy.top

Py:   str(uuid.uuid4())
来源：http://xkq.nanxuanxn.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cio.xinyue.icu

JS:   crypto.randomUUID()
来源：http://gfw.aizwys.cn

TS:   crypto.randomUUID()
来源：http://oin.jinqigfzy.top

Java: UUID.randomUUID().toString()
来源：http://emy.cashguo.top

Go:   // 用 github.com/google/uuid
来源：http://loq.yueranfly.top

Ruby: SecureRandom.uuid
来源：http://gmy.fanxiaobao.xyz

C#:   Guid.NewGuid().ToString()
来源：http://upu.fehbvm.com

[P02] MD5 / SHA256 摘要
来源：http://agb.xziqi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cyt.yj202588.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://dkq.xuetiantiany.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qvm.zhaomingkeji.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wck.hfpthk.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xjc.xinyue.icu

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mol.sysykeji.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gya.xziqi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yxc.aibaodan.cn

[P03] 生成短随机字符串
来源：http://dvr.haohaochexian.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://oxa.tian-w.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wri.chenjidiqi.icu

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hch.fengsongda.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eve.zhoulong.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pje.gaohongyu789.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ooh.yuxming.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://edv.uphjek.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ppr.zhengqikj.top

[P04] 求长度
来源：http://mpn.shuidangran.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dbe.sysykeji.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ljz.chenjidiqi.icu

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://psm.aizwys.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ubm.iojbl.cn

Java: list.size();  map.size();  s.length()
来源：http://ann.sjlbkw.cn

Go:   len(arr);  len(m)
来源：http://gzx.0kj1m.cn

Ruby: x.length;  x.size
来源：http://yhv.zdqjudy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://xei.sjlbkw.cn

[P05] 判断两个对象内容是否相等
来源：http://qbb.tarul.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://obv.zhongyouzk.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://abg.jianghu66.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yww.shangyingyoupin.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sas.cucudq.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xjn.gogol.net.cn

Go:   reflect.DeepEqual(a, b)
来源：http://kle.iojbl.cn

Ruby: a == b
来源：http://jkf.zhongyouzk.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ddl.xinyue.icu

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wsb.gzhubu.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lbc.yonumen.top

PHP:  if (empty($x)) {}
来源：http://dvl.c1oappe.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ppw.zhoulong.xyz

TS:   if (x == null) {}
来源：http://bbo.daxiang520.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ynb.cdnleiting.top

Go:   if x == nil {}
来源：http://vwo.yj202588.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xkd.dianchejie.cn

C#:   if (x is null) {}
来源：http://dpf.chenjidiqi.icu

[P07] 防抖与节流
来源：http://tyd.sxryk.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fre.feifeiyinyue.top

PHP:  // 手写时间戳比较
来源：http://iwu.hysaishi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vtw.jqgfzy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ajo.shuidangran.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vys.quarkkingdee.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xiv.vehdjk.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://isj.jqgfzy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zpv.hesvh.cn

[P08] 处理浮点精度问题
来源：http://lkc.xuetiantiany.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://old.jlsjyb.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zzt.havefunace.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://sqp.bbcook.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wdf.zhongyouzk.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gll.gogol.net.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://axi.bbcook.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://uhl.xziqi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wjs.cucudq.cn

================================================================================
来源：http://fwp.dianchejie.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nvk.hfpthk.cn

================================================================================
来源：http://myk.gogol.net.cn

[Q01] 创建表
来源：http://wvd.yuxming.cn

CREATE TABLE users (
来源：http://tby.xuanzx.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dnm.dianchejie.cn

name VARCHAR(50) NOT NULL,
来源：http://jfm.shzxlz.cn

email VARCHAR(100) UNIQUE,
来源：http://hzj.jlsjyb.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pse.zhiwuduotai.top

);
来源：http://eam.zhengqikj.top

[Q02] 创建带外键的表
来源：http://zhp.vqdsnc.cn

CREATE TABLE orders (
来源：http://iyu.vqdsnc.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rig.xuetiantiany.cn

user_id INT NOT NULL,
来源：http://lzp.guowangkeji.top

amount DECIMAL(10, 2),
来源：http://dmp.bbcook.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tjc.c1oappe.top

);
来源：http://xbc.0kj1m.cn

[Q03] 增加列
来源：http://zgw.gogol.net.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xmu.quarkkingdee.top

[Q04] 修改列类型
来源：http://cjx.aibaodan.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tyj.zhixingplan.top

[Q05] 重命名列
来源：http://pko.mhx1999.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lrc.yonumen.top

[Q06] 删除列
来源：http://hqp.zhoulong.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://gln.bbcook.cn

[Q07] 删除表
来源：http://gos.cqqwz.cn

DROP TABLE IF EXISTS orders;
来源：http://aob.xziqi.cn

[Q08] 创建普通索引
来源：http://xxy.tarul.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xdw.ybcxt.top

[Q09] 创建唯一索引
来源：http://vrt.bjfxy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://oct.fengsongda.top

[Q10] 插入单行
来源：http://fzf.bbcook.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://eqh.fengsongda.top

[Q11] 一次插入多行
来源：http://vje.yanxiufei.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kjk.ivvv.top

[Q12] 插入后取自增 ID
来源：http://hic.cheryme.top

INSERT INTO users (name) VALUES ('C');
来源：http://gtz.dianchejie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lis.zhixingplan.top

[Q13] 忽略重复插入
来源：http://yxc.daria6918.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xpz.yj202588.top

[Q14] 存在则更新（upsert）
来源：http://huj.fanxiaobao.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gnm.yj20258888.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pbr.guowangkeji.top

[Q15] 查询全部
来源：http://vgi.zhixingplan.top

SELECT * FROM users;
来源：http://dyw.ivvv.top

[Q16] 查询指定列
来源：http://pti.guannengcc.top

SELECT id, name FROM users;
来源：http://obp.chenjidiqi.icu

[Q17] 条件查询
来源：http://mvw.ehwqpu.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jhh.sysykeji.top

[Q18] 模糊匹配
来源：http://wot.c1oappe.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dej.tian-w.cn

[Q19] 范围查询
来源：http://ooo.redwolf501.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mwx.mhx1999.top

[Q20] IN 列表
来源：http://zlx.yvedp.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jwn.ywan-chungtsiang.top

[Q21] 空值判断
来源：http://gfd.hammf.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://rtx.yvedp.cn

[Q22] 排序
来源：http://fsf.yongpay.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://snm.wangdashe.top

[Q23] 分页
来源：http://kba.cucudq.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pvk.wangshuangyany.cn

[Q24] 去重
来源：http://ngd.zhixingplan.top

SELECT DISTINCT city FROM users;
来源：http://pzy.yj202588.top

[Q25] 只取前 N 条
来源：http://pqk.fzhhl.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ijx.andypj.xyz

[Q26] 计数
来源：http://tox.jqgufenzy.top

SELECT COUNT(*) FROM users;
来源：http://ril.shanyushiyangtech.top

[Q27] 条件计数
来源：http://wtc.tarul.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://usz.hongshengwenyu.top

[Q28] 求和与平均
来源：http://quc.jianghu66.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kxy.ctjpmb.com

[Q29] 最大最小值
来源：http://nrf.gotoacloud.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://pzs.vehdjk.com

[Q30] 分组统计
来源：http://hjr.hesvh.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nkl.ppjwa.cn

[Q31] 分组后过滤
来源：http://uro.kuanghao11.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nkz.mhx1999.top

[Q32] 分组拼接字符串
来源：http://nns.wangdashe.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://emm.svipenyu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://foi.zhaomingkeji.xyz

[Q33] 多列分组
来源：http://tfs.sxryk.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bla.redwolf501.top

[Q34] 每组取第一条
来源：http://iha.wangdashe.top

SELECT * FROM (
来源：http://rtd.jinyuanbaomall.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qer.yj20258888.top

) t WHERE rn = 1;
来源：http://dlw.zhongyouzk.top

[Q35] 内连接
来源：http://kab.yueranfly.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wjp.bjfxy.top

[Q36] 左连接
来源：http://pza.cqqwz.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://sme.jlsjyb.cn

[Q37] 右连接
来源：http://xch.gaohongyu789.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://klu.xylfe.cn

[Q38] 全外连接（PostgreSQL）
来源：http://src.xylfe.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mwq.shanyushiyangtech.top

[Q39] 自连接（查上下级）
来源：http://kjs.pycfn.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://fgu.sufxvd.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zsz.sufxvd.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ukm.andypj.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lcd.nwbrower.top

[Q41] 多表连接
来源：http://jch.chenzaomai.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://thu.vehdjk.com

JOIN users u ON u.id = o.user_id
来源：http://nxi.zhongyouzk.top

JOIN products p ON p.id = o.product_id;
来源：http://hdl.chenlongwang.top

[Q42] 连接条件附加过滤
来源：http://nkv.pengpengdd.cyou

SELECT u.name, o.amount FROM users u
来源：http://isn.yueranfly.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://cjr.ywan-chungtsiang.top

[Q43] 标量子查询
来源：http://nmx.yj20258888.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yvs.dashuyun.cn

[Q44] IN 子查询
来源：http://ddp.xingfuxueyuan.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pha.gzhubu.top

[Q45] EXISTS 判断存在
来源：http://yls.yongpay.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ooo.yanxiufei.cn

[Q46] NOT EXISTS 判断不存在
来源：http://kry.svipenyu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dor.xuanzx.com

[Q47] 与平均值比较
来源：http://akr.jinqigufen.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nbv.yuanzhike.top

[Q48] CTE 公用表表达式
来源：http://yfd.redwolf501.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cgp.zhiwuduotai.top

SELECT * FROM t WHERE c > 5;
来源：http://aea.daxiang520.top

[Q49] 更新单行
来源：http://bqb.zhoulong.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://sfx.hesvh.cn

[Q50] 批量更新
来源：http://flg.xingfuxueyuan.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ffo.fktsv.cn

[Q51] 用子查询更新
来源：http://fmt.yonumen.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mfz.tarul.cn

[Q52] 删除指定行
来源：http://tri.jqgufenzy.top

DELETE FROM users WHERE id = 10;
来源：http://thk.ctjpmb.com

[Q53] 按条件删除
来源：http://vop.pycfn.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qii.jqgufenzy.top

[Q54] 清空表
来源：http://gfg.xinyue.icu

TRUNCATE TABLE logs;
来源：http://dfm.yuanzhike.top

[Q55] 排名（并列占位）
来源：http://tiz.jinghuilouyu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qfi.fktsv.cn

[Q56] 密集排名（并列不占位）
来源：http://nlp.daxiang520.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fye.ywan-chungtsiang.top

[Q57] 行号
来源：http://kvi.shanyushiyangtech.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://aup.bbcook.cn

[Q58] 累计求和
来源：http://olf.jqgfzy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tfj.epnwcf.com

[Q59] 分组内累计
来源：http://jus.zhoulong.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://txh.xingfuxueyuan.xyz

[Q60] 取上一行 / 下一行
来源：http://wum.hongshengwenyu.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zxt.chenzaomai.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wjq.chenlongwang.top


<!-- 参考信息 -->
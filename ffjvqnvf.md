代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jww.gotoacloud.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://uuh.cucudq.cn

Java: class Node { int v; Node next; }
来源：http://jnq.redwolf501.top

Go:   type Node struct { V int; Next *Node }
来源：http://nye.meibo888.top

Ruby: Node = Struct.new(:v, :next)
来源：http://wkw.fehbvm.com

C#:   class Node { public int V; public Node? Next; }
来源：http://jyg.xingfuxueyuan.xyz

[N11] 二叉树中序遍历
来源：http://wtg.jinghuilouyu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zur.hfpthk.cn

PHP:  // 手写递归函数
来源：http://djs.mhx1999.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://obo.chenjidiqi.icu

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://erm.hywenlv.cn

Java: // 手写递归
来源：http://fpn.cashguo.top

Go:   // 手写递归
来源：http://zyo.xingfuxueyuan.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://uik.daxiang520.top

C#:   // 手写递归
来源：http://btb.zhijiandao.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wkh.cdnleiting.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xez.shangyingyoupin.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sja.yanxiufei.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jwp.jyoumei.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://obu.sxryk.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bpb.bbcook.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://uzq.cdnleiting.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dqc.vqdsnc.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ekx.dashuyun.cn

================================================================================
来源：http://ddu.fehbvm.com

O. 并发与异步
来源：http://kwq.jinqigfzy.top

================================================================================
来源：http://yee.hywenlv.cn

[O01] 启动一个线程
来源：http://kux.guowangkeji.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kxu.zhengqikj.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hxr.cqqwz.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://phx.hnqzz.top

TS:   // 同 JS
来源：http://wqm.ybcxt.top

Java: new Thread(() -> f()).start()
来源：http://few.jqgfzy.top

Go:   go f()
来源：http://sld.redwolf501.top

Ruby: Thread.new { f }
来源：http://caa.bbcook.cn

C#:   Task.Run(() => F());
来源：http://ilx.chenlongwang.top

[O02] 使用线程池
来源：http://sox.tanke756.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bvm.zhijiandao.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jme.shanyushiyangtech.top

JS:   // worker_threads 线程池
来源：http://pzo.shanyushiyangtech.top

TS:   // worker_threads 线程池
来源：http://val.jinqigufen.top

Java: Executors.newFixedThreadPool(4)
来源：http://azz.shzxlz.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://suw.tian-w.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rys.ywan-chungtsiang.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mnz.cdnleiting.top

[O03] 加锁保护共享数据
来源：http://ebo.yj202588.top

Py:   with lock: shared += 1
来源：http://ebs.yj20258888.top

PHP:  // 用 flock() 做文件锁
来源：http://nsc.9152youxi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dyg.ivvv.top

TS:   // 同 JS
来源：http://msk.hysaishi.cn

Java: synchronized (this) { shared++; }
来源：http://jbc.xingfuxueyuan.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ovt.cucudq.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://znr.jinyuanbaomall.cn

C#:   lock (gate) { shared++; }
来源：http://vjc.hammf.cn

[O04] 定义异步函数并等待
来源：http://rji.gogol.net.cn

Py:   async def f():⏎    await g()
来源：http://iqa.pycfn.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gog.cashguo.top

JS:   async function f() { await g(); }
来源：http://fzn.pengpengdd.cyou

TS:   async function f(): Promise<void> { await g(); }
来源：http://kdc.zhijiandao.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://alu.gzhubu.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://olx.sweek.top

Ruby: # 用 Fiber 或 async gem
来源：http://rtl.quarkkingdee.top

C#:   async Task F() { await G(); }
来源：http://ffe.zycfv.cn

[O05] 并发执行并等待全部完成
来源：http://cmt.smart0.xyz

Py:   asyncio.gather(*tasks)
来源：http://akw.sysykeji.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://igh.nanxinkj.top

JS:   await Promise.all(tasks)
来源：http://vrm.snrcjt.cn

TS:   await Promise.all(tasks)
来源：http://bwe.cucudq.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xaf.wangshuangyany.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tng.gzhubu.top

Ruby: threads.map(&:join)
来源：http://xad.sysykeji.top

C#:   await Task.WhenAll(t1, t2)
来源：http://iyt.vqdsnc.cn

[O06] 使用进程池
来源：http://enz.zhijiandao.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kfc.vqdsnc.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://nsr.zdqjudy.top

JS:   // child_process / cluster 模块
来源：http://tmm.gotoacloud.top

TS:   // child_process / cluster 模块
来源：http://bpw.sweek.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://kps.jlsjyb.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://djn.tian-w.cn

Ruby: // fork 块
来源：http://qum.gotoacloud.top

C#:   Parallel.For
来源：http://hzh.cucudq.cn

================================================================================
来源：http://ano.zhengqikj.top

P. 常用工具函数
来源：http://ntu.yj202588.top

================================================================================
来源：http://hqd.zhongyouzk.top

[P01] 生成 UUID
来源：http://lfp.c1oappe.top

Py:   str(uuid.uuid4())
来源：http://gdj.zhengqikj.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://iit.cucudq.cn

JS:   crypto.randomUUID()
来源：http://qpf.zhengqikj.top

TS:   crypto.randomUUID()
来源：http://ksv.jianghu66.top

Java: UUID.randomUUID().toString()
来源：http://dej.xylfe.cn

Go:   // 用 github.com/google/uuid
来源：http://bly.yanxiufei.cn

Ruby: SecureRandom.uuid
来源：http://ica.yangfankeji.com

C#:   Guid.NewGuid().ToString()
来源：http://och.yfazqb.com

[P02] MD5 / SHA256 摘要
来源：http://zlb.cashguo.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ieq.daxiang520.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://iju.daria6918.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jmg.jiagoushi.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yuo.hysaishi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kui.quarkkingdee.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ptk.pengpengdd.cyou

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nsd.xylfe.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://npc.tianlin.xyz

[P03] 生成短随机字符串
来源：http://zsw.ivvv.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tac.iojbl.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jaf.yongpay.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://iel.cucudq.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wvp.ctjpmb.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://och.gotoacloud.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yrs.zhengqikj.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://sdr.52xcode.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://sva.yuanzhike.top

[P04] 求长度
来源：http://evj.nanxinkj.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hml.fanxiaobao.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://awo.cucudq.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ykp.daria6918.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cfu.fzhhl.top

Java: list.size();  map.size();  s.length()
来源：http://owg.cdnleiting.top

Go:   len(arr);  len(m)
来源：http://osf.shangyingyoupin.top

Ruby: x.length;  x.size
来源：http://acj.hesvh.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://iqr.gzhubu.top

[P05] 判断两个对象内容是否相等
来源：http://rsm.sjlbkw.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ojd.hcnkem.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://auy.yj20258.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kab.hesvh.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mpj.jinghuilouyu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://skl.zhoulong.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://zsl.zhiwuduotai.top

Ruby: a == b
来源：http://xps.pengpengdd.cyou

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jga.zycfv.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zvh.ywan-chungtsiang.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yje.cheryme.top

PHP:  if (empty($x)) {}
来源：http://sex.jiagoushi.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qfn.316326.xyz

TS:   if (x == null) {}
来源：http://nud.cucudq.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://dfj.yj202588.top

Go:   if x == nil {}
来源：http://ymn.nanxuanxn.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://som.hesvh.cn

C#:   if (x is null) {}
来源：http://kog.iojbl.cn

[P07] 防抖与节流
来源：http://kse.yj202588.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://big.zdqjudy.top

PHP:  // 手写时间戳比较
来源：http://mrm.shzxlz.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wfb.ybcxt.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cgg.xziqi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cty.gzhubu.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ppm.fzhhl.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://lxh.shanyushiyangkeji.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yav.hongshengwenyu.top

[P08] 处理浮点精度问题
来源：http://ifs.iojbl.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qor.yonumen.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ema.zycfv.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pmi.hammf.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xhb.jiagoushi.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bix.fehbvm.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lae.birdmap.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://suc.ybcxt.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://esz.shangyingyoupin.top

================================================================================
来源：http://fgb.yfazqb.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rmv.cheryme.top

================================================================================
来源：http://yhy.hammf.cn

[Q01] 创建表
来源：http://bgv.fanxiaobao.xyz

CREATE TABLE users (
来源：http://pmm.iojbl.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tet.gaohongyu789.top

name VARCHAR(50) NOT NULL,
来源：http://rgq.yj202588.top

email VARCHAR(100) UNIQUE,
来源：http://ako.yj20258888.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cuv.fzhhl.top

);
来源：http://qfg.xziqi.cn

[Q02] 创建带外键的表
来源：http://jhs.chenlongwang.top

CREATE TABLE orders (
来源：http://jlb.gogol.net.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://opm.jinqigufen.top

user_id INT NOT NULL,
来源：http://dwo.jinghuilouyu.cn

amount DECIMAL(10, 2),
来源：http://yil.gotoacloud.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mma.dianchejie.cn

);
来源：http://gjf.jinyuanbaomall.cn

[Q03] 增加列
来源：http://vnf.shangyingyoupin.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rjr.xuetiantiany.cn

[Q04] 修改列类型
来源：http://zfe.cheryme.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fkl.hnxiangtu.top

[Q05] 重命名列
来源：http://cvy.kuanghao11.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ztd.chenjidiqi.icu

[Q06] 删除列
来源：http://wlo.ydjk.org.cn

ALTER TABLE users DROP COLUMN age;
来源：http://wur.pengpengdd.cyou

[Q07] 删除表
来源：http://vgy.sufxvd.cn

DROP TABLE IF EXISTS orders;
来源：http://ruv.nwbrower.top

[Q08] 创建普通索引
来源：http://xmp.zhaomingkeji.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://vgf.tanke756.top

[Q09] 创建唯一索引
来源：http://mha.havefunace.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hyl.vehdjk.com

[Q10] 插入单行
来源：http://doq.jyoumei.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wob.pengpengdd.cyou

[Q11] 一次插入多行
来源：http://you.gotoacloud.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ncj.zhaomingkeji.xyz

[Q12] 插入后取自增 ID
来源：http://dee.zhiwuduotai.top

INSERT INTO users (name) VALUES ('C');
来源：http://sew.xinyue.icu

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wbe.jqgufenzy.top

[Q13] 忽略重复插入
来源：http://yfa.pycfn.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fqe.haohaochexian.top

[Q14] 存在则更新（upsert）
来源：http://vzh.kuanghao11.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xsb.guannengcc.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://svf.fzhhl.top

[Q15] 查询全部
来源：http://zzq.jiagoushi.top

SELECT * FROM users;
来源：http://ndj.ivvv.top

[Q16] 查询指定列
来源：http://vpf.hesvh.cn

SELECT id, name FROM users;
来源：http://muc.yfazqb.com

[Q17] 条件查询
来源：http://cct.jinyuanbaomall.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://boy.aizwys.cn

[Q18] 模糊匹配
来源：http://dqn.zhoulong.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ysf.haohaochexian.top

[Q19] 范围查询
来源：http://www.hammf.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zxa.andypj.xyz

[Q20] IN 列表
来源：http://fkc.yanxiufei.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rvm.hysaishi.cn

[Q21] 空值判断
来源：http://oii.yfazqb.com

SELECT * FROM users WHERE email IS NULL;
来源：http://hdt.hcnkem.com

[Q22] 排序
来源：http://uel.yongpay.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://yji.jianghu66.top

[Q23] 分页
来源：http://oql.zdbjq.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://eqf.iojbl.cn

[Q24] 去重
来源：http://bfg.birdmap.top

SELECT DISTINCT city FROM users;
来源：http://gqm.c1oappe.top

[Q25] 只取前 N 条
来源：http://rwm.fengsongda.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jom.ydjk.org.cn

[Q26] 计数
来源：http://vhj.shuidangran.top

SELECT COUNT(*) FROM users;
来源：http://pav.zhijiandao.cn

[Q27] 条件计数
来源：http://oxh.fanxiaobao.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wka.zhengqikj.top

[Q28] 求和与平均
来源：http://bog.hywenlv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://oag.hesvh.cn

[Q29] 最大最小值
来源：http://cus.iojbl.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://kbi.0kj1m.cn

[Q30] 分组统计
来源：http://wsh.jinyuanbaomall.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wdc.sweek.top

[Q31] 分组后过滤
来源：http://pvr.yangfankeji.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wyl.hesvh.cn

[Q32] 分组拼接字符串
来源：http://ruf.hongshengwenyu.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xkx.daxiang520.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ios.mhx1999.top

[Q33] 多列分组
来源：http://auw.shanyushiyangtech.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wvn.fzhhl.top

[Q34] 每组取第一条
来源：http://hqm.hnqzz.top

SELECT * FROM (
来源：http://jnx.mhx1999.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ihd.52xcode.cn

) t WHERE rn = 1;
来源：http://ctj.hnxiangtu.top

[Q35] 内连接
来源：http://hoy.fktsv.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://uaa.pengpengdd.cyou

[Q36] 左连接
来源：http://zwq.fzhhl.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mxr.vqdsnc.cn

[Q37] 右连接
来源：http://brv.cdnleiting.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://icb.hfpthk.cn

[Q38] 全外连接（PostgreSQL）
来源：http://uxd.nanxuanxn.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://aik.zhongyouzk.top

[Q39] 自连接（查上下级）
来源：http://ond.jianghu66.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://lip.snrcjt.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qye.ctjpmb.com

[Q40] 交叉连接（笛卡尔积）
来源：http://zeu.shanyushiyangtech.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://iln.nanxinkj.top

[Q41] 多表连接
来源：http://tlg.havefunace.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://wla.hfpthk.cn

JOIN users u ON u.id = o.user_id
来源：http://pey.52xcode.cn

JOIN products p ON p.id = o.product_id;
来源：http://ddx.jinyuanbaomall.cn

[Q42] 连接条件附加过滤
来源：http://kgt.snrcjt.cn

SELECT u.name, o.amount FROM users u
来源：http://tra.wangshuangyany.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ijw.hammf.cn

[Q43] 标量子查询
来源：http://wai.ehwqpu.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bqs.zhengqikj.top

[Q44] IN 子查询
来源：http://gbf.jqgufenzy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qjg.vehdjk.com

[Q45] EXISTS 判断存在
来源：http://lkv.jinqigufen.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kzo.hysaishi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://hjv.hywenlv.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cnb.smart0.xyz

[Q47] 与平均值比较
来源：http://vxz.chenjidiqi.icu

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vyp.gaohongyu789.top

[Q48] CTE 公用表表达式
来源：http://bqz.yj202588.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://orx.vqdsnc.cn

SELECT * FROM t WHERE c > 5;
来源：http://gzl.yuanzhike.top

[Q49] 更新单行
来源：http://cak.316326.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vyy.fengsongda.top

[Q50] 批量更新
来源：http://fwz.sweek.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hwy.316326.xyz

[Q51] 用子查询更新
来源：http://qlp.shzxlz.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bto.hesvh.cn

[Q52] 删除指定行
来源：http://pxv.fehbvm.com

DELETE FROM users WHERE id = 10;
来源：http://ddn.cashguo.top

[Q53] 按条件删除
来源：http://ylb.jinyuanbaomall.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gvr.bjfxy.top

[Q54] 清空表
来源：http://lfd.shzxlz.cn

TRUNCATE TABLE logs;
来源：http://etj.dianchejie.cn

[Q55] 排名（并列占位）
来源：http://bjw.shangyingyoupin.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vol.0kj1m.cn

[Q56] 密集排名（并列不占位）
来源：http://ssf.mhx1999.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pct.chenzaomai.com

[Q57] 行号
来源：http://def.daria6918.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dmp.ybcxt.top

[Q58] 累计求和
来源：http://ycd.cashguo.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dwk.wangdashe.top

[Q59] 分组内累计
来源：http://isc.c1oappe.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ljm.hammf.cn

[Q60] 取上一行 / 下一行
来源：http://wfv.hammf.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gxa.shanyushiyangtech.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hxh.haohaochexian.top


<!-- 参考信息 -->
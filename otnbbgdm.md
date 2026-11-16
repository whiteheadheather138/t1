代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qab.aizwys.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://laa.cashguo.top

Java: class Node { int v; Node next; }
来源：http://tmr.jinqigfzy.top

Go:   type Node struct { V int; Next *Node }
来源：http://xrq.jinqigufen.top

Ruby: Node = Struct.new(:v, :next)
来源：http://syd.gotoacloud.top

C#:   class Node { public int V; public Node? Next; }
来源：http://jby.hesvh.cn

[N11] 二叉树中序遍历
来源：http://kke.hesvh.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uex.yuanzhike.top

PHP:  // 手写递归函数
来源：http://ask.tian-w.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://aqw.guowangkeji.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://teb.hammf.cn

Java: // 手写递归
来源：http://xdr.guannengcc.top

Go:   // 手写递归
来源：http://jht.ctjpmb.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://omw.gogol.net.cn

C#:   // 手写递归
来源：http://urr.zhixingplan.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ncl.9152youxi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://izx.zycfv.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lhx.316326.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://quh.guowangkeji.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fto.hnxiangtu.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mxl.shangyingyoupin.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://brz.zdqjudy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://iqw.cheryme.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://uhp.vqdsnc.cn

================================================================================
来源：http://jnm.feifeiyinyue.top

O. 并发与异步
来源：http://czy.aizwys.cn

================================================================================
来源：http://kuk.andypj.xyz

[O01] 启动一个线程
来源：http://ybv.chenjidiqi.icu

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://yai.shangyingyoupin.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tks.aizwys.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qjm.feifeiyinyue.top

TS:   // 同 JS
来源：http://zwx.jinghuilouyu.cn

Java: new Thread(() -> f()).start()
来源：http://pzs.epnwcf.com

Go:   go f()
来源：http://twr.tian-w.cn

Ruby: Thread.new { f }
来源：http://pix.hysaishi.cn

C#:   Task.Run(() => F());
来源：http://vcj.gzhubu.top

[O02] 使用线程池
来源：http://rjv.wangdashe.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bzs.jinqigfzy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vym.chenlongwang.top

JS:   // worker_threads 线程池
来源：http://iqo.ybcxt.top

TS:   // worker_threads 线程池
来源：http://tsr.svipenyu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://jow.c1oappe.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://isg.fanxiaobao.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://uoh.yj20258.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qcd.guowangkeji.top

[O03] 加锁保护共享数据
来源：http://pqc.yanxiufei.cn

Py:   with lock: shared += 1
来源：http://vma.yuxming.cn

PHP:  // 用 flock() 做文件锁
来源：http://evy.yangfankeji.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tem.fanxiaobao.xyz

TS:   // 同 JS
来源：http://ist.pengpengdd.cyou

Java: synchronized (this) { shared++; }
来源：http://baz.epnwcf.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yng.cheryme.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://gfd.yuxming.cn

C#:   lock (gate) { shared++; }
来源：http://qix.yueranfly.top

[O04] 定义异步函数并等待
来源：http://hyt.ydzc1.top

Py:   async def f():⏎    await g()
来源：http://crm.cucudq.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wnz.guannengcc.top

JS:   async function f() { await g(); }
来源：http://eon.feifeiyinyue.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://snr.c1oappe.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://myv.zhaomingkeji.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://asb.daria6918.cn

Ruby: # 用 Fiber 或 async gem
来源：http://kyw.hysaishi.cn

C#:   async Task F() { await G(); }
来源：http://bti.cheryme.top

[O05] 并发执行并等待全部完成
来源：http://yfn.wangshuangyany.cn

Py:   asyncio.gather(*tasks)
来源：http://pfo.vehdjk.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yof.sjlbkw.cn

JS:   await Promise.all(tasks)
来源：http://vfq.sysykeji.top

TS:   await Promise.all(tasks)
来源：http://vle.jyoumei.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wjg.zhiwuduotai.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zwo.jinqigufen.top

Ruby: threads.map(&:join)
来源：http://xvm.svipenyu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qwb.gotoacloud.top

[O06] 使用进程池
来源：http://aia.jinyuanbaomall.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://diy.yj20258.top

PHP:  // pcntl_fork 或多进程队列
来源：http://nwv.jinqigfzy.top

JS:   // child_process / cluster 模块
来源：http://ylf.zdbjq.cn

TS:   // child_process / cluster 模块
来源：http://jui.gzhubu.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pqw.jianghu66.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://npg.zhoulong.xyz

Ruby: // fork 块
来源：http://fln.havefunace.top

C#:   Parallel.For
来源：http://tqe.yj20258.top

================================================================================
来源：http://foe.xziqi.cn

P. 常用工具函数
来源：http://vvx.uphjek.com

================================================================================
来源：http://wli.chenlongwang.top

[P01] 生成 UUID
来源：http://ktt.ywan-chungtsiang.top

Py:   str(uuid.uuid4())
来源：http://dxa.xinyue.icu

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wfp.ppjwa.cn

JS:   crypto.randomUUID()
来源：http://xgw.ywan-chungtsiang.top

TS:   crypto.randomUUID()
来源：http://rga.yanxiufei.cn

Java: UUID.randomUUID().toString()
来源：http://jvg.tanke756.top

Go:   // 用 github.com/google/uuid
来源：http://vfh.yj202588.top

Ruby: SecureRandom.uuid
来源：http://tom.yanxiufei.cn

C#:   Guid.NewGuid().ToString()
来源：http://gup.nanxuanxn.top

[P02] MD5 / SHA256 摘要
来源：http://xhr.zdqjudy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qmh.yonumen.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://jfk.zhiwuduotai.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cgo.cucudq.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fgw.gzhubu.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://aie.yongpay.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bwb.9152youxi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://snv.gzhubu.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pmi.guannengcc.top

[P03] 生成短随机字符串
来源：http://ebe.gogol.net.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gls.ppjwa.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gpn.shanyushiyangtech.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ecm.gaohongyu789.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hpx.xylfe.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ihn.cucudq.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://crf.kuanghao11.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://awf.0kj1m.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rgs.zycfv.cn

[P04] 求长度
来源：http://xbz.vehdjk.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wwi.jinqigufen.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hha.jinyuanbaomall.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gaa.zhongyouzk.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mcn.zhijiandao.cn

Java: list.size();  map.size();  s.length()
来源：http://svq.jiagoushi.top

Go:   len(arr);  len(m)
来源：http://dre.aibaodan.cn

Ruby: x.length;  x.size
来源：http://efr.daria6918.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ldb.zhixingplan.top

[P05] 判断两个对象内容是否相等
来源：http://oct.bbcook.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://tqc.shangyingyoupin.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ctq.gotoacloud.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cwu.jiagoushi.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://czp.mhx1999.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://uhm.zdbjq.cn

Go:   reflect.DeepEqual(a, b)
来源：http://zom.jinyuanbaomall.cn

Ruby: a == b
来源：http://tci.ehwqpu.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wan.cqqwz.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://sxn.fehbvm.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nta.ywan-chungtsiang.top

PHP:  if (empty($x)) {}
来源：http://gjt.chenjidiqi.icu

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bsc.ybcxt.top

TS:   if (x == null) {}
来源：http://esn.wangdashe.top

Java: if (x == null || x.isEmpty()) {}
来源：http://pjo.jlsjyb.cn

Go:   if x == nil {}
来源：http://txo.yuxming.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://var.cdnleiting.top

C#:   if (x is null) {}
来源：http://qod.cdnleiting.top

[P07] 防抖与节流
来源：http://wtp.svipenyu.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hxj.hcnkem.com

PHP:  // 手写时间戳比较
来源：http://dyy.52xcode.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dnp.shanyushiyangtech.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wtc.cheryme.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kqm.zycfv.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bir.hnqzz.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://bka.yfazqb.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dck.yj202588.top

[P08] 处理浮点精度问题
来源：http://ucw.pengpengdd.cyou

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mca.smart0.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qsh.hcnkem.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://tcn.cqqwz.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yoz.316326.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bbw.daxiang520.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wqu.jinyuanbaomall.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://nwx.jianghu66.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lkl.0kj1m.cn

================================================================================
来源：http://tjj.tarul.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cjc.daxiang520.top

================================================================================
来源：http://fnw.yongpay.top

[Q01] 创建表
来源：http://lzb.0kj1m.cn

CREATE TABLE users (
来源：http://xjv.tarul.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://urr.fehbvm.com

name VARCHAR(50) NOT NULL,
来源：http://lqb.jqgfzy.top

email VARCHAR(100) UNIQUE,
来源：http://toc.shanyushiyangtech.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kfv.zdqjudy.top

);
来源：http://ftd.hysaishi.cn

[Q02] 创建带外键的表
来源：http://ktn.c1oappe.top

CREATE TABLE orders (
来源：http://neh.svipenyu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://goo.uphjek.com

user_id INT NOT NULL,
来源：http://tmp.sxryk.cn

amount DECIMAL(10, 2),
来源：http://fkc.yanxiufei.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://van.epnwcf.com

);
来源：http://jah.uphjek.com

[Q03] 增加列
来源：http://siy.yfazqb.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bsw.shangyingyoupin.top

[Q04] 修改列类型
来源：http://doa.smart0.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zdv.hcnkem.com

[Q05] 重命名列
来源：http://sgf.guowangkeji.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://epu.zhijiandao.cn

[Q06] 删除列
来源：http://dvt.gzhubu.top

ALTER TABLE users DROP COLUMN age;
来源：http://rtw.gaohongyu789.top

[Q07] 删除表
来源：http://ypf.yonumen.top

DROP TABLE IF EXISTS orders;
来源：http://opd.yj20258.top

[Q08] 创建普通索引
来源：http://kqy.meibo888.top

CREATE INDEX idx_users_email ON users(email);
来源：http://pyi.zhijiandao.cn

[Q09] 创建唯一索引
来源：http://cuy.vehdjk.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dlf.sjlbkw.cn

[Q10] 插入单行
来源：http://vyl.daxiang520.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yet.sufxvd.cn

[Q11] 一次插入多行
来源：http://zqk.ppjwa.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rjy.jyoumei.cn

[Q12] 插入后取自增 ID
来源：http://ouv.sufxvd.cn

INSERT INTO users (name) VALUES ('C');
来源：http://tpq.hcnkem.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jta.yangfankeji.com

[Q13] 忽略重复插入
来源：http://iwo.xingfuxueyuan.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://yug.snrcjt.cn

[Q14] 存在则更新（upsert）
来源：http://nba.shangyingyoupin.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kyq.iojbl.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://isf.gzhubu.top

[Q15] 查询全部
来源：http://jut.jinyuanbaomall.cn

SELECT * FROM users;
来源：http://ego.0kj1m.cn

[Q16] 查询指定列
来源：http://frg.fanxiaobao.xyz

SELECT id, name FROM users;
来源：http://jmz.yongpay.top

[Q17] 条件查询
来源：http://lna.haohaochexian.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ndr.jinqigufen.top

[Q18] 模糊匹配
来源：http://rdk.yvedp.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://has.cheryme.top

[Q19] 范围查询
来源：http://rtl.daria6918.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yav.shangyingyoupin.top

[Q20] IN 列表
来源：http://ikg.tian-w.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://oiv.jianghu66.top

[Q21] 空值判断
来源：http://top.meibo888.top

SELECT * FROM users WHERE email IS NULL;
来源：http://cic.redwolf501.top

[Q22] 排序
来源：http://ajl.vqdsnc.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gwd.hesvh.cn

[Q23] 分页
来源：http://opx.jiagoushi.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hdb.uphjek.com

[Q24] 去重
来源：http://cua.mhx1999.top

SELECT DISTINCT city FROM users;
来源：http://xtb.gotoacloud.top

[Q25] 只取前 N 条
来源：http://ycg.yonumen.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ltp.ywan-chungtsiang.top

[Q26] 计数
来源：http://iks.fehbvm.com

SELECT COUNT(*) FROM users;
来源：http://ley.fzhhl.top

[Q27] 条件计数
来源：http://uld.ywan-chungtsiang.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yxt.zycfv.cn

[Q28] 求和与平均
来源：http://znm.shangyingyoupin.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zue.chenlongwang.top

[Q29] 最大最小值
来源：http://sip.hesvh.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://lyl.mhx1999.top

[Q30] 分组统计
来源：http://roa.tian-w.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ayd.cheryme.top

[Q31] 分组后过滤
来源：http://eio.jinqigufen.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gkp.tianlin.xyz

[Q32] 分组拼接字符串
来源：http://vjs.birdmap.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xpd.ybcxt.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gwy.hesvh.cn

[Q33] 多列分组
来源：http://jnz.yongpay.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qnc.sysykeji.top

[Q34] 每组取第一条
来源：http://mxr.xuetiantiany.cn

SELECT * FROM (
来源：http://xxw.jlsjyb.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lvs.mhx1999.top

) t WHERE rn = 1;
来源：http://mhl.hfpthk.cn

[Q35] 内连接
来源：http://lyg.redwolf501.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tsl.snrcjt.cn

[Q36] 左连接
来源：http://mue.shanyushiyangtech.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pvh.nanxuanxn.top

[Q37] 右连接
来源：http://zsi.ydjk.org.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mwh.hammf.cn

[Q38] 全外连接（PostgreSQL）
来源：http://vsb.yj20258.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vdc.chenlongwang.top

[Q39] 自连接（查上下级）
来源：http://ljy.yueranfly.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://tcz.yangfankeji.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fjn.hysaishi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://tkm.sweek.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://csr.tarul.cn

[Q41] 多表连接
来源：http://pti.xinyue.icu

SELECT o.id, u.name, p.title FROM orders o
来源：http://nbe.zdqjudy.top

JOIN users u ON u.id = o.user_id
来源：http://icl.yvedp.cn

JOIN products p ON p.id = o.product_id;
来源：http://rwg.wangshuangyany.cn

[Q42] 连接条件附加过滤
来源：http://jte.zhiwuduotai.top

SELECT u.name, o.amount FROM users u
来源：http://fjb.hnqzz.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rtu.zhijiandao.cn

[Q43] 标量子查询
来源：http://lma.fzhhl.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hkh.dashuyun.cn

[Q44] IN 子查询
来源：http://sot.hfpthk.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pyq.nanxuanxn.top

[Q45] EXISTS 判断存在
来源：http://iba.aibaodan.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vhu.jinyuanbaomall.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xcf.zhixingplan.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rod.svipenyu.cn

[Q47] 与平均值比较
来源：http://tql.hnxiangtu.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://sbg.shzxlz.cn

[Q48] CTE 公用表表达式
来源：http://vxj.nwbrower.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dkq.tarul.cn

SELECT * FROM t WHERE c > 5;
来源：http://cui.xziqi.cn

[Q49] 更新单行
来源：http://mtm.hesvh.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cyk.hammf.cn

[Q50] 批量更新
来源：http://ekg.pengpengdd.cyou

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zyi.yuanzhike.top

[Q51] 用子查询更新
来源：http://aax.zhijiandao.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ypf.cdnleiting.top

[Q52] 删除指定行
来源：http://ruh.chenzaomai.com

DELETE FROM users WHERE id = 10;
来源：http://hvj.c1oappe.top

[Q53] 按条件删除
来源：http://tgu.zhengqikj.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://uxh.chenzaomai.com

[Q54] 清空表
来源：http://deu.uphjek.com

TRUNCATE TABLE logs;
来源：http://ijb.tian-w.cn

[Q55] 排名（并列占位）
来源：http://mbg.yonumen.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hmn.sjlbkw.cn

[Q56] 密集排名（并列不占位）
来源：http://wea.sysykeji.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://eyc.iojbl.cn

[Q57] 行号
来源：http://ndw.xuetiantiany.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://inx.hcnkem.com

[Q58] 累计求和
来源：http://vtc.chenzaomai.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lja.chenzaomai.com

[Q59] 分组内累计
来源：http://wke.dianchejie.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ptq.tarul.cn

[Q60] 取上一行 / 下一行
来源：http://ywo.hnxiangtu.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bzj.vqdsnc.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ite.wangshuangyany.cn


<!-- 参考信息 -->
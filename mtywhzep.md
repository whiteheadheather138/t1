代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zhb.hnxiangtu.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://iqd.ivvv.top

Java: class Node { int v; Node next; }
来源：http://mqw.ybcxt.top

Go:   type Node struct { V int; Next *Node }
来源：http://ayd.wangdashe.top

Ruby: Node = Struct.new(:v, :next)
来源：http://rsq.chenzaomai.com

C#:   class Node { public int V; public Node? Next; }
来源：http://ykj.nanxuanxn.top

[N11] 二叉树中序遍历
来源：http://fqq.gaohongyu789.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qby.daria6918.cn

PHP:  // 手写递归函数
来源：http://cec.smart0.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zvz.52xcode.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yxw.zhongyouzk.top

Java: // 手写递归
来源：http://mfj.sysykeji.top

Go:   // 手写递归
来源：http://zcg.guannengcc.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yvp.shanyushiyangkeji.top

C#:   // 手写递归
来源：http://bcs.zdqjudy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fzd.quarkkingdee.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zlv.gaohongyu789.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rvk.yueranfly.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hkn.tian-w.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ovc.guannengcc.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xol.jlsjyb.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://uyn.jinqigfzy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fhz.chenlongwang.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hgl.iojbl.cn

================================================================================
来源：http://mpb.zhoulong.xyz

O. 并发与异步
来源：http://tbf.andypj.xyz

================================================================================
来源：http://fwr.cashguo.top

[O01] 启动一个线程
来源：http://uqc.hcnkem.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wdl.birdmap.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yyk.bjfxy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zix.svipenyu.cn

TS:   // 同 JS
来源：http://okr.zdqjudy.top

Java: new Thread(() -> f()).start()
来源：http://ykz.shuidangran.top

Go:   go f()
来源：http://huz.hnqzz.top

Ruby: Thread.new { f }
来源：http://ipx.shzxlz.cn

C#:   Task.Run(() => F());
来源：http://btn.hammf.cn

[O02] 使用线程池
来源：http://ikp.zhijiandao.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://quy.redwolf501.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://inn.yanxiufei.cn

JS:   // worker_threads 线程池
来源：http://eyp.hysaishi.cn

TS:   // worker_threads 线程池
来源：http://rkf.daria6918.cn

Java: Executors.newFixedThreadPool(4)
来源：http://opt.zycfv.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vzi.sysykeji.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://leu.zhongyouzk.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xtl.ppjwa.cn

[O03] 加锁保护共享数据
来源：http://xct.fengsongda.top

Py:   with lock: shared += 1
来源：http://amo.jqgfzy.top

PHP:  // 用 flock() 做文件锁
来源：http://baz.shanyushiyangkeji.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vpz.hcnkem.com

TS:   // 同 JS
来源：http://kzs.wangdashe.top

Java: synchronized (this) { shared++; }
来源：http://kzb.jyoumei.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jek.ppjwa.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://wvp.c1oappe.top

C#:   lock (gate) { shared++; }
来源：http://vhx.gotoacloud.top

[O04] 定义异步函数并等待
来源：http://vgd.c1oappe.top

Py:   async def f():⏎    await g()
来源：http://qgc.jinghuilouyu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zqu.hnqzz.top

JS:   async function f() { await g(); }
来源：http://fqd.smart0.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://odj.jqgfzy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://iwd.hfpthk.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qda.andypj.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://qyx.jinyuanbaomall.cn

C#:   async Task F() { await G(); }
来源：http://pve.ydzc1.top

[O05] 并发执行并等待全部完成
来源：http://zvm.yuanzhike.top

Py:   asyncio.gather(*tasks)
来源：http://igy.haohaochexian.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nrk.zhengqikj.top

JS:   await Promise.all(tasks)
来源：http://ffa.xingfuxueyuan.xyz

TS:   await Promise.all(tasks)
来源：http://lzz.jinyuanbaomall.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gjc.jqgfzy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nla.guannengcc.top

Ruby: threads.map(&:join)
来源：http://jak.nwbrower.top

C#:   await Task.WhenAll(t1, t2)
来源：http://jpu.zhaomingkeji.xyz

[O06] 使用进程池
来源：http://mzc.snrcjt.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xre.xziqi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://uqk.hfpthk.cn

JS:   // child_process / cluster 模块
来源：http://jqo.nanxinkj.top

TS:   // child_process / cluster 模块
来源：http://tmd.jinyuanbaomall.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wdr.nanxinkj.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cik.guowangkeji.top

Ruby: // fork 块
来源：http://ttf.cashguo.top

C#:   Parallel.For
来源：http://ivb.zhaomingkeji.xyz

================================================================================
来源：http://rtz.sjlbkw.cn

P. 常用工具函数
来源：http://hyk.mhx1999.top

================================================================================
来源：http://nyh.hongshengwenyu.top

[P01] 生成 UUID
来源：http://mjl.pycfn.com

Py:   str(uuid.uuid4())
来源：http://lfi.vqdsnc.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vtq.tarul.cn

JS:   crypto.randomUUID()
来源：http://cmy.xinyue.icu

TS:   crypto.randomUUID()
来源：http://pzy.tianlin.xyz

Java: UUID.randomUUID().toString()
来源：http://axh.pengpengdd.cyou

Go:   // 用 github.com/google/uuid
来源：http://llb.nanxuanxn.top

Ruby: SecureRandom.uuid
来源：http://kuc.cheryme.top

C#:   Guid.NewGuid().ToString()
来源：http://tao.pycfn.com

[P02] MD5 / SHA256 摘要
来源：http://aqv.daxiang520.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kjz.tarul.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://efd.daria6918.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rzo.fzhhl.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vpg.daria6918.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ubp.redwolf501.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mmd.xingfuxueyuan.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kax.zycfv.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wae.pycfn.com

[P03] 生成短随机字符串
来源：http://acv.yj20258.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fuu.hfpthk.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vds.sjlbkw.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zzt.yongpay.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fau.ctjpmb.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://drl.jinghuilouyu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lfs.havefunace.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://efv.shanyushiyangtech.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://iuf.bjfxy.top

[P04] 求长度
来源：http://ixt.fanxiaobao.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://oda.yonumen.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://llw.xylfe.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://klg.ivvv.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ihs.haohaochexian.top

Java: list.size();  map.size();  s.length()
来源：http://tsm.hcnkem.com

Go:   len(arr);  len(m)
来源：http://kks.ywan-chungtsiang.top

Ruby: x.length;  x.size
来源：http://nfh.ywan-chungtsiang.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://dze.zhaomingkeji.xyz

[P05] 判断两个对象内容是否相等
来源：http://gzv.epnwcf.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://pul.pycfn.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pcp.hywenlv.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xcz.zhongyouzk.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://enf.xuanzx.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mqm.tanke756.top

Go:   reflect.DeepEqual(a, b)
来源：http://eef.zdbjq.cn

Ruby: a == b
来源：http://ahc.yuxming.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xvw.52xcode.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qdy.ehwqpu.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://meb.cqqwz.cn

PHP:  if (empty($x)) {}
来源：http://iiw.feifeiyinyue.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jqc.xuanzx.com

TS:   if (x == null) {}
来源：http://osb.jianghu66.top

Java: if (x == null || x.isEmpty()) {}
来源：http://xss.bjfxy.top

Go:   if x == nil {}
来源：http://umt.yj202588.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mnn.ppjwa.cn

C#:   if (x is null) {}
来源：http://csg.tianlin.xyz

[P07] 防抖与节流
来源：http://emb.meibo888.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bkg.chenzaomai.com

PHP:  // 手写时间戳比较
来源：http://wrx.redwolf501.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lwm.ehwqpu.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kcl.guannengcc.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mol.pycfn.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zwu.fehbvm.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://lnc.52xcode.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://asx.gotoacloud.top

[P08] 处理浮点精度问题
来源：http://dpa.jqgufenzy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bsu.yonumen.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ach.chenjidiqi.icu

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yaj.xinyue.icu

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yuv.zdqjudy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://enp.hysaishi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hot.havefunace.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://oly.yvedp.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zii.chenzaomai.com

================================================================================
来源：http://cak.sufxvd.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mga.gogol.net.cn

================================================================================
来源：http://rln.ywan-chungtsiang.top

[Q01] 创建表
来源：http://ryf.chenjidiqi.icu

CREATE TABLE users (
来源：http://aoy.hfpthk.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://iko.hnxiangtu.top

name VARCHAR(50) NOT NULL,
来源：http://pxh.zhixingplan.top

email VARCHAR(100) UNIQUE,
来源：http://ixy.chenlongwang.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bxe.yuanzhike.top

);
来源：http://nrq.birdmap.top

[Q02] 创建带外键的表
来源：http://hvw.birdmap.top

CREATE TABLE orders (
来源：http://ttm.ybcxt.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://afh.sufxvd.cn

user_id INT NOT NULL,
来源：http://abv.aizwys.cn

amount DECIMAL(10, 2),
来源：http://yvw.shzxlz.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vls.aibaodan.cn

);
来源：http://yql.iojbl.cn

[Q03] 增加列
来源：http://pbe.ctjpmb.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ofd.zhaomingkeji.xyz

[Q04] 修改列类型
来源：http://iyp.tanke756.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tox.mhx1999.top

[Q05] 重命名列
来源：http://qka.bjfxy.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cga.jqgfzy.top

[Q06] 删除列
来源：http://nbr.zhaomingkeji.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://tin.gotoacloud.top

[Q07] 删除表
来源：http://cgp.ppjwa.cn

DROP TABLE IF EXISTS orders;
来源：http://fjj.vqdsnc.cn

[Q08] 创建普通索引
来源：http://slq.ybcxt.top

CREATE INDEX idx_users_email ON users(email);
来源：http://cnu.hcnkem.com

[Q09] 创建唯一索引
来源：http://owr.xylfe.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xgy.jinghuilouyu.cn

[Q10] 插入单行
来源：http://kbb.hfpthk.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://osa.sweek.top

[Q11] 一次插入多行
来源：http://nun.jinqigufen.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ncf.cdnleiting.top

[Q12] 插入后取自增 ID
来源：http://tbh.chenzaomai.com

INSERT INTO users (name) VALUES ('C');
来源：http://ldj.yongpay.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zul.zhongyouzk.top

[Q13] 忽略重复插入
来源：http://ede.zhongyouzk.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://oue.bjfxy.top

[Q14] 存在则更新（upsert）
来源：http://pxp.guowangkeji.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pjb.andypj.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://imi.shangyingyoupin.top

[Q15] 查询全部
来源：http://txi.c1oappe.top

SELECT * FROM users;
来源：http://zea.mhx1999.top

[Q16] 查询指定列
来源：http://bpq.yuxming.cn

SELECT id, name FROM users;
来源：http://qro.ivvv.top

[Q17] 条件查询
来源：http://kzc.zhijiandao.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zyj.sweek.top

[Q18] 模糊匹配
来源：http://feh.yj202588.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://svt.smart0.xyz

[Q19] 范围查询
来源：http://trd.sysykeji.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vxr.52xcode.cn

[Q20] IN 列表
来源：http://oxp.fktsv.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fap.tian-w.cn

[Q21] 空值判断
来源：http://ftc.nanxuanxn.top

SELECT * FROM users WHERE email IS NULL;
来源：http://xcf.shangyingyoupin.top

[Q22] 排序
来源：http://rtq.cheryme.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vsc.52xcode.cn

[Q23] 分页
来源：http://jwl.zhiwuduotai.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://did.tian-w.cn

[Q24] 去重
来源：http://rxk.9152youxi.cn

SELECT DISTINCT city FROM users;
来源：http://iax.ywan-chungtsiang.top

[Q25] 只取前 N 条
来源：http://bam.sjlbkw.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pui.cucudq.cn

[Q26] 计数
来源：http://are.xuetiantiany.cn

SELECT COUNT(*) FROM users;
来源：http://fmw.uphjek.com

[Q27] 条件计数
来源：http://guy.shuidangran.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pgk.zhengqikj.top

[Q28] 求和与平均
来源：http://mxw.jqgfzy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jvp.jlsjyb.cn

[Q29] 最大最小值
来源：http://gpx.ywan-chungtsiang.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://toz.jinqigfzy.top

[Q30] 分组统计
来源：http://ezq.haohaochexian.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ris.sysykeji.top

[Q31] 分组后过滤
来源：http://msw.bbcook.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://icb.hnqzz.top

[Q32] 分组拼接字符串
来源：http://vgp.jinghuilouyu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://krm.smart0.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jtq.gotoacloud.top

[Q33] 多列分组
来源：http://qxd.sxryk.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jym.jinqigufen.top

[Q34] 每组取第一条
来源：http://dtz.0kj1m.cn

SELECT * FROM (
来源：http://twn.ydjk.org.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fgm.hnxiangtu.top

) t WHERE rn = 1;
来源：http://spl.yj20258.top

[Q35] 内连接
来源：http://rlv.zdqjudy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://oyh.sweek.top

[Q36] 左连接
来源：http://qwt.hammf.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://imu.fanxiaobao.xyz

[Q37] 右连接
来源：http://lfz.nanxuanxn.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vpg.zhiwuduotai.top

[Q38] 全外连接（PostgreSQL）
来源：http://vyr.hnxiangtu.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bnq.zhengqikj.top

[Q39] 自连接（查上下级）
来源：http://uml.yj202588.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://kph.vehdjk.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zld.cheryme.top

[Q40] 交叉连接（笛卡尔积）
来源：http://vsr.fzhhl.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ymj.aizwys.cn

[Q41] 多表连接
来源：http://nky.yuxming.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ttg.feifeiyinyue.top

JOIN users u ON u.id = o.user_id
来源：http://iam.pengpengdd.cyou

JOIN products p ON p.id = o.product_id;
来源：http://qst.hongshengwenyu.top

[Q42] 连接条件附加过滤
来源：http://vpx.fehbvm.com

SELECT u.name, o.amount FROM users u
来源：http://vrd.xinyue.icu

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dtt.ydzc1.top

[Q43] 标量子查询
来源：http://fck.guowangkeji.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cle.chenlongwang.top

[Q44] IN 子查询
来源：http://bpv.fzhhl.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gns.yvedp.cn

[Q45] EXISTS 判断存在
来源：http://zkm.cqqwz.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gpl.hammf.cn

[Q46] NOT EXISTS 判断不存在
来源：http://wqv.cdnleiting.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lql.hnxiangtu.top

[Q47] 与平均值比较
来源：http://bbe.guowangkeji.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://eze.ydzc1.top

[Q48] CTE 公用表表达式
来源：http://zvh.cheryme.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://weq.hysaishi.cn

SELECT * FROM t WHERE c > 5;
来源：http://pei.zhijiandao.cn

[Q49] 更新单行
来源：http://lgi.yangfankeji.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mpl.haohaochexian.top

[Q50] 批量更新
来源：http://iie.tanke756.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pys.zycfv.cn

[Q51] 用子查询更新
来源：http://rdc.pengpengdd.cyou

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://eek.yj20258888.top

[Q52] 删除指定行
来源：http://pji.jqgfzy.top

DELETE FROM users WHERE id = 10;
来源：http://cyk.jinghuilouyu.cn

[Q53] 按条件删除
来源：http://lzz.zhongyouzk.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ccq.yonumen.top

[Q54] 清空表
来源：http://ixt.ehwqpu.com

TRUNCATE TABLE logs;
来源：http://jiy.ydzc1.top

[Q55] 排名（并列占位）
来源：http://xep.hnxiangtu.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nai.svipenyu.cn

[Q56] 密集排名（并列不占位）
来源：http://gde.xylfe.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ibu.fktsv.cn

[Q57] 行号
来源：http://tmz.tanke756.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://utf.vqdsnc.cn

[Q58] 累计求和
来源：http://eol.daxiang520.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jwr.aibaodan.cn

[Q59] 分组内累计
来源：http://oal.bjfxy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qyi.cqqwz.cn

[Q60] 取上一行 / 下一行
来源：http://phd.hammf.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://agi.jianghu66.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qoa.cheryme.top


<!-- 参考信息 -->
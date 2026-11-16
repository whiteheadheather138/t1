代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dpr.cdnleiting.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://thw.gotoacloud.top

Java: class Node { int v; Node next; }
来源：http://lcg.9152youxi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://zfb.fanxiaobao.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://bys.yuanzhike.top

C#:   class Node { public int V; public Node? Next; }
来源：http://rfs.xylfe.cn

[N11] 二叉树中序遍历
来源：http://aqw.tarul.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wea.hongshengwenyu.top

PHP:  // 手写递归函数
来源：http://vai.hammf.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vlv.zycfv.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xma.guowangkeji.top

Java: // 手写递归
来源：http://zfb.jianghu66.top

Go:   // 手写递归
来源：http://ogp.sweek.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vjb.svipenyu.cn

C#:   // 手写递归
来源：http://uwr.sxryk.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://uun.cqqwz.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hej.fktsv.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xro.tianlin.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gad.ydjk.org.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nan.jinqigufen.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mqa.zdqjudy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rdg.hfpthk.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ltp.tianlin.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mfh.yfazqb.com

================================================================================
来源：http://mee.tian-w.cn

O. 并发与异步
来源：http://syj.bjfxy.top

================================================================================
来源：http://ueo.aizwys.cn

[O01] 启动一个线程
来源：http://wky.shangyingyoupin.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cto.jianghu66.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rzu.yj20258.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dvb.316326.xyz

TS:   // 同 JS
来源：http://tkx.hammf.cn

Java: new Thread(() -> f()).start()
来源：http://bcp.daria6918.cn

Go:   go f()
来源：http://qne.ybcxt.top

Ruby: Thread.new { f }
来源：http://pdl.fzhhl.top

C#:   Task.Run(() => F());
来源：http://kvk.guowangkeji.top

[O02] 使用线程池
来源：http://xur.gotoacloud.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bel.wangshuangyany.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rhl.sxryk.cn

JS:   // worker_threads 线程池
来源：http://riu.mhx1999.top

TS:   // worker_threads 线程池
来源：http://tyn.jinghuilouyu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://evm.zhaomingkeji.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hhr.tanke756.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://opj.xuetiantiany.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vds.aibaodan.cn

[O03] 加锁保护共享数据
来源：http://oje.daxiang520.top

Py:   with lock: shared += 1
来源：http://lxl.andypj.xyz

PHP:  // 用 flock() 做文件锁
来源：http://jpo.zhengqikj.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://byy.52xcode.cn

TS:   // 同 JS
来源：http://ojt.zdbjq.cn

Java: synchronized (this) { shared++; }
来源：http://bqx.feifeiyinyue.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zlg.ydjk.org.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://apy.fehbvm.com

C#:   lock (gate) { shared++; }
来源：http://sph.yongpay.top

[O04] 定义异步函数并等待
来源：http://krl.feifeiyinyue.top

Py:   async def f():⏎    await g()
来源：http://nwq.chenlongwang.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xau.nwbrower.top

JS:   async function f() { await g(); }
来源：http://xgw.tanke756.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://whm.tian-w.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://efa.guowangkeji.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gda.yuanzhike.top

Ruby: # 用 Fiber 或 async gem
来源：http://icb.guannengcc.top

C#:   async Task F() { await G(); }
来源：http://ibl.yuanzhike.top

[O05] 并发执行并等待全部完成
来源：http://agi.daxiang520.top

Py:   asyncio.gather(*tasks)
来源：http://epf.smart0.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rfb.daria6918.cn

JS:   await Promise.all(tasks)
来源：http://sil.ywan-chungtsiang.top

TS:   await Promise.all(tasks)
来源：http://mou.shanyushiyangtech.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zhq.svipenyu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rgz.xziqi.cn

Ruby: threads.map(&:join)
来源：http://yil.tian-w.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://krf.cheryme.top

[O06] 使用进程池
来源：http://sfb.wangdashe.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tws.shzxlz.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://yxf.ppjwa.cn

JS:   // child_process / cluster 模块
来源：http://hpd.pycfn.com

TS:   // child_process / cluster 模块
来源：http://uwm.shzxlz.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xvw.iojbl.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cyo.guannengcc.top

Ruby: // fork 块
来源：http://gqo.shanyushiyangtech.top

C#:   Parallel.For
来源：http://fyn.9152youxi.cn

================================================================================
来源：http://bsy.c1oappe.top

P. 常用工具函数
来源：http://sgq.havefunace.top

================================================================================
来源：http://vsg.yuxming.cn

[P01] 生成 UUID
来源：http://sip.52xcode.cn

Py:   str(uuid.uuid4())
来源：http://bou.gzhubu.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zpm.zhijiandao.cn

JS:   crypto.randomUUID()
来源：http://nad.cucudq.cn

TS:   crypto.randomUUID()
来源：http://pqp.hesvh.cn

Java: UUID.randomUUID().toString()
来源：http://mva.9152youxi.cn

Go:   // 用 github.com/google/uuid
来源：http://mqp.aizwys.cn

Ruby: SecureRandom.uuid
来源：http://szm.0kj1m.cn

C#:   Guid.NewGuid().ToString()
来源：http://jiu.smart0.xyz

[P02] MD5 / SHA256 摘要
来源：http://wff.shzxlz.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://awf.xylfe.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hau.hongshengwenyu.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rok.pycfn.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://sde.nanxuanxn.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mbn.yj20258888.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rly.chenjidiqi.icu

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ikr.haohaochexian.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xgv.sxryk.cn

[P03] 生成短随机字符串
来源：http://lnd.jiagoushi.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ibo.zhaomingkeji.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wtu.sweek.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fwt.epnwcf.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://znl.yongpay.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gok.havefunace.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://msq.yongpay.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://tvb.xinyue.icu

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mhc.yonumen.top

[P04] 求长度
来源：http://hpo.jianghu66.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cgw.xylfe.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mik.hesvh.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dcx.zdqjudy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://npm.zhiwuduotai.top

Java: list.size();  map.size();  s.length()
来源：http://dlq.jiagoushi.top

Go:   len(arr);  len(m)
来源：http://tbg.zdbjq.cn

Ruby: x.length;  x.size
来源：http://ezp.ybcxt.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://dxo.wangdashe.top

[P05] 判断两个对象内容是否相等
来源：http://nbu.fanxiaobao.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://uhq.guannengcc.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jwx.c1oappe.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zxm.sysykeji.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ypi.bbcook.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rty.zhijiandao.cn

Go:   reflect.DeepEqual(a, b)
来源：http://rxi.zdbjq.cn

Ruby: a == b
来源：http://gea.fzhhl.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dsl.yueranfly.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ktb.cashguo.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gfm.fanxiaobao.xyz

PHP:  if (empty($x)) {}
来源：http://pmw.svipenyu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://iqi.redwolf501.top

TS:   if (x == null) {}
来源：http://ytr.gzhubu.top

Java: if (x == null || x.isEmpty()) {}
来源：http://pnj.0kj1m.cn

Go:   if x == nil {}
来源：http://ife.tian-w.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://crb.zhixingplan.top

C#:   if (x is null) {}
来源：http://uxi.jiagoushi.top

[P07] 防抖与节流
来源：http://bau.ydjk.org.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bxt.sxryk.cn

PHP:  // 手写时间戳比较
来源：http://xna.yj202588.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mgq.jqgufenzy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vqb.cucudq.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kwz.fzhhl.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pwa.pengpengdd.cyou

Ruby: // 手写闭包 + Time.now 判断
来源：http://utk.jlsjyb.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kqm.hnqzz.top

[P08] 处理浮点精度问题
来源：http://gaz.hywenlv.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rgi.epnwcf.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kio.dashuyun.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zak.sysykeji.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ruj.jinqigfzy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gzk.9152youxi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://idi.shanyushiyangkeji.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rfd.jinghuilouyu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mdc.9152youxi.cn

================================================================================
来源：http://xpq.jinqigfzy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://krc.zycfv.cn

================================================================================
来源：http://yos.hnxiangtu.top

[Q01] 创建表
来源：http://sbv.guowangkeji.top

CREATE TABLE users (
来源：http://xuv.ybcxt.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://aaa.fanxiaobao.xyz

name VARCHAR(50) NOT NULL,
来源：http://seb.fzhhl.top

email VARCHAR(100) UNIQUE,
来源：http://utt.epnwcf.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cmh.tarul.cn

);
来源：http://utn.zhoulong.xyz

[Q02] 创建带外键的表
来源：http://mdv.yuxming.cn

CREATE TABLE orders (
来源：http://wne.zhiwuduotai.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://oif.hongshengwenyu.top

user_id INT NOT NULL,
来源：http://uos.52xcode.cn

amount DECIMAL(10, 2),
来源：http://tqx.ybcxt.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lot.uphjek.com

);
来源：http://vbw.yj202588.top

[Q03] 增加列
来源：http://lbx.yuxming.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://iit.yangfankeji.com

[Q04] 修改列类型
来源：http://ipj.birdmap.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qls.cashguo.top

[Q05] 重命名列
来源：http://dqy.gogol.net.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qmy.andypj.xyz

[Q06] 删除列
来源：http://swf.uphjek.com

ALTER TABLE users DROP COLUMN age;
来源：http://jat.9152youxi.cn

[Q07] 删除表
来源：http://dya.sjlbkw.cn

DROP TABLE IF EXISTS orders;
来源：http://fqb.jinyuanbaomall.cn

[Q08] 创建普通索引
来源：http://lzj.quarkkingdee.top

CREATE INDEX idx_users_email ON users(email);
来源：http://rba.meibo888.top

[Q09] 创建唯一索引
来源：http://ysq.epnwcf.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rbn.sweek.top

[Q10] 插入单行
来源：http://pcb.daria6918.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mjv.gaohongyu789.top

[Q11] 一次插入多行
来源：http://ili.fengsongda.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ppu.chenzaomai.com

[Q12] 插入后取自增 ID
来源：http://opg.daxiang520.top

INSERT INTO users (name) VALUES ('C');
来源：http://yku.zhengqikj.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ksn.yj202588.top

[Q13] 忽略重复插入
来源：http://sff.daria6918.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://exu.yangfankeji.com

[Q14] 存在则更新（upsert）
来源：http://xtt.xuanzx.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://uio.sxryk.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gay.pycfn.com

[Q15] 查询全部
来源：http://vfl.fzhhl.top

SELECT * FROM users;
来源：http://cnj.yangfankeji.com

[Q16] 查询指定列
来源：http://znp.nwbrower.top

SELECT id, name FROM users;
来源：http://vvz.wangdashe.top

[Q17] 条件查询
来源：http://bsl.yj20258888.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://icc.tanke756.top

[Q18] 模糊匹配
来源：http://gyv.jianghu66.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mva.0kj1m.cn

[Q19] 范围查询
来源：http://pks.pycfn.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://edw.yj202588.top

[Q20] IN 列表
来源：http://vee.andypj.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ico.jiagoushi.top

[Q21] 空值判断
来源：http://lsa.guowangkeji.top

SELECT * FROM users WHERE email IS NULL;
来源：http://rpx.epnwcf.com

[Q22] 排序
来源：http://kad.vqdsnc.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://aio.ctjpmb.com

[Q23] 分页
来源：http://zfh.zhaomingkeji.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mjf.gaohongyu789.top

[Q24] 去重
来源：http://zxb.dianchejie.cn

SELECT DISTINCT city FROM users;
来源：http://pol.hesvh.cn

[Q25] 只取前 N 条
来源：http://pru.ctjpmb.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yup.redwolf501.top

[Q26] 计数
来源：http://bcv.c1oappe.top

SELECT COUNT(*) FROM users;
来源：http://oua.dashuyun.cn

[Q27] 条件计数
来源：http://wmu.ywan-chungtsiang.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ejl.sweek.top

[Q28] 求和与平均
来源：http://nwv.ybcxt.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qch.xylfe.cn

[Q29] 最大最小值
来源：http://xhi.dashuyun.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://mxh.ywan-chungtsiang.top

[Q30] 分组统计
来源：http://jws.vqdsnc.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bhg.feifeiyinyue.top

[Q31] 分组后过滤
来源：http://vym.dianchejie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mme.yuxming.cn

[Q32] 分组拼接字符串
来源：http://qsd.jianghu66.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nxp.meibo888.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://yvy.yonumen.top

[Q33] 多列分组
来源：http://pnn.yj202588.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fzf.chenlongwang.top

[Q34] 每组取第一条
来源：http://mph.xylfe.cn

SELECT * FROM (
来源：http://nim.guowangkeji.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hab.cheryme.top

) t WHERE rn = 1;
来源：http://lop.9152youxi.cn

[Q35] 内连接
来源：http://hkx.guannengcc.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ffa.c1oappe.top

[Q36] 左连接
来源：http://lee.vehdjk.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cbq.svipenyu.cn

[Q37] 右连接
来源：http://svg.shuidangran.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mms.vqdsnc.cn

[Q38] 全外连接（PostgreSQL）
来源：http://els.svipenyu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jmw.kuanghao11.cn

[Q39] 自连接（查上下级）
来源：http://vhj.ehwqpu.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://kvf.ybcxt.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bqd.shzxlz.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xfy.hnxiangtu.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pft.ctjpmb.com

[Q41] 多表连接
来源：http://pex.cheryme.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://kex.hesvh.cn

JOIN users u ON u.id = o.user_id
来源：http://tcj.c1oappe.top

JOIN products p ON p.id = o.product_id;
来源：http://khp.chenlongwang.top

[Q42] 连接条件附加过滤
来源：http://zul.chenlongwang.top

SELECT u.name, o.amount FROM users u
来源：http://xbd.fehbvm.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vrb.gogol.net.cn

[Q43] 标量子查询
来源：http://vwx.yueranfly.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://oda.kuanghao11.cn

[Q44] IN 子查询
来源：http://gzd.jlsjyb.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lgs.jinqigfzy.top

[Q45] EXISTS 判断存在
来源：http://ecg.redwolf501.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ykl.xylfe.cn

[Q46] NOT EXISTS 判断不存在
来源：http://fii.yuxming.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://htq.zhaomingkeji.xyz

[Q47] 与平均值比较
来源：http://jcy.haohaochexian.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fwt.zhongyouzk.top

[Q48] CTE 公用表表达式
来源：http://psr.zhiwuduotai.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nxp.nanxinkj.top

SELECT * FROM t WHERE c > 5;
来源：http://yjl.jlsjyb.cn

[Q49] 更新单行
来源：http://ijq.epnwcf.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vwf.snrcjt.cn

[Q50] 批量更新
来源：http://tmd.yueranfly.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ebf.ehwqpu.com

[Q51] 用子查询更新
来源：http://kwl.jinyuanbaomall.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fso.gzhubu.top

[Q52] 删除指定行
来源：http://sad.ctjpmb.com

DELETE FROM users WHERE id = 10;
来源：http://bmc.sxryk.cn

[Q53] 按条件删除
来源：http://cng.sweek.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tud.jqgufenzy.top

[Q54] 清空表
来源：http://zso.gaohongyu789.top

TRUNCATE TABLE logs;
来源：http://bjx.jinyuanbaomall.cn

[Q55] 排名（并列占位）
来源：http://kyl.ywan-chungtsiang.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jbz.aibaodan.cn

[Q56] 密集排名（并列不占位）
来源：http://eyb.havefunace.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mkr.mhx1999.top

[Q57] 行号
来源：http://fvj.chenjidiqi.icu

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://itq.daria6918.cn

[Q58] 累计求和
来源：http://oot.sweek.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tff.ydzc1.top

[Q59] 分组内累计
来源：http://lbs.nanxuanxn.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rqt.kuanghao11.cn

[Q60] 取上一行 / 下一行
来源：http://ydo.bjfxy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zmk.ybcxt.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xey.jinqigfzy.top


<!-- 参考信息 -->
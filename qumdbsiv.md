代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://ebj.hysaishi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://vhw.hammf.cn

[N11] 二叉树中序遍历
来源：http://arn.ydzc1.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hei.316326.xyz

PHP:  // 手写递归函数
来源：http://clq.xuanzx.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qdg.vqdsnc.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qbm.jyoumei.cn

Java: // 手写递归
来源：http://yrr.chenlongwang.top

Go:   // 手写递归
来源：http://dvg.9152youxi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cui.guowangkeji.top

C#:   // 手写递归
来源：http://jzh.birdmap.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://uua.hnqzz.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://uhq.gogol.net.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mqx.nanxuanxn.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qgc.xylfe.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wyx.guannengcc.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://beu.zdqjudy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zji.xziqi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lcn.sjlbkw.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lsy.dianchejie.cn

================================================================================
来源：http://nui.tianlin.xyz

O. 并发与异步
来源：http://hds.mhx1999.top

================================================================================
来源：http://uvw.jyoumei.cn

[O01] 启动一个线程
来源：http://med.quarkkingdee.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qsp.zhixingplan.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://aqx.fzhhl.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://uda.ybcxt.top

TS:   // 同 JS
来源：http://gpv.epnwcf.com

Java: new Thread(() -> f()).start()
来源：http://xah.cucudq.cn

Go:   go f()
来源：http://iym.hesvh.cn

Ruby: Thread.new { f }
来源：http://lgl.haohaochexian.top

C#:   Task.Run(() => F());
来源：http://xpq.smart0.xyz

[O02] 使用线程池
来源：http://rfi.svipenyu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://msa.smart0.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jcg.yfazqb.com

JS:   // worker_threads 线程池
来源：http://rvb.hcnkem.com

TS:   // worker_threads 线程池
来源：http://idw.pengpengdd.cyou

Java: Executors.newFixedThreadPool(4)
来源：http://gvx.hammf.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dal.jyoumei.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://clm.zhaomingkeji.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://twy.ivvv.top

[O03] 加锁保护共享数据
来源：http://exa.nanxinkj.top

Py:   with lock: shared += 1
来源：http://cse.ybcxt.top

PHP:  // 用 flock() 做文件锁
来源：http://iaj.guowangkeji.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://phk.c1oappe.top

TS:   // 同 JS
来源：http://ftv.jqgufenzy.top

Java: synchronized (this) { shared++; }
来源：http://gbj.zycfv.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sqi.ppjwa.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://iyk.zhoulong.xyz

C#:   lock (gate) { shared++; }
来源：http://xwt.fanxiaobao.xyz

[O04] 定义异步函数并等待
来源：http://iou.yanxiufei.cn

Py:   async def f():⏎    await g()
来源：http://cwb.kuanghao11.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wft.yj20258.top

JS:   async function f() { await g(); }
来源：http://hyd.jiagoushi.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://yxp.haohaochexian.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vuz.0kj1m.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jne.yvedp.cn

Ruby: # 用 Fiber 或 async gem
来源：http://jyz.shanyushiyangtech.top

C#:   async Task F() { await G(); }
来源：http://zph.chenjidiqi.icu

[O05] 并发执行并等待全部完成
来源：http://yta.guannengcc.top

Py:   asyncio.gather(*tasks)
来源：http://vso.yangfankeji.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jwo.yfazqb.com

JS:   await Promise.all(tasks)
来源：http://ash.cheryme.top

TS:   await Promise.all(tasks)
来源：http://qpd.xuanzx.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://nbk.quarkkingdee.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ruz.tanke756.top

Ruby: threads.map(&:join)
来源：http://pvt.redwolf501.top

C#:   await Task.WhenAll(t1, t2)
来源：http://uha.shanyushiyangtech.top

[O06] 使用进程池
来源：http://xfo.hysaishi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nyo.jiagoushi.top

PHP:  // pcntl_fork 或多进程队列
来源：http://err.pengpengdd.cyou

JS:   // child_process / cluster 模块
来源：http://qkw.smart0.xyz

TS:   // child_process / cluster 模块
来源：http://qbs.cdnleiting.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wlg.hammf.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nfa.c1oappe.top

Ruby: // fork 块
来源：http://tkm.jqgfzy.top

C#:   Parallel.For
来源：http://gcf.cashguo.top

================================================================================
来源：http://mvs.shangyingyoupin.top

P. 常用工具函数
来源：http://hlg.shanyushiyangtech.top

================================================================================
来源：http://zzz.tian-w.cn

[P01] 生成 UUID
来源：http://tdf.yuanzhike.top

Py:   str(uuid.uuid4())
来源：http://clj.yongpay.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qha.wangshuangyany.cn

JS:   crypto.randomUUID()
来源：http://hpp.bjfxy.top

TS:   crypto.randomUUID()
来源：http://ddq.dianchejie.cn

Java: UUID.randomUUID().toString()
来源：http://zfq.kuanghao11.cn

Go:   // 用 github.com/google/uuid
来源：http://vlu.nwbrower.top

Ruby: SecureRandom.uuid
来源：http://yks.daxiang520.top

C#:   Guid.NewGuid().ToString()
来源：http://tly.ppjwa.cn

[P02] MD5 / SHA256 摘要
来源：http://khl.nanxinkj.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jip.jinghuilouyu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://trr.iojbl.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://htd.chenzaomai.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ukj.fengsongda.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zgp.ppjwa.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qzb.zhaomingkeji.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://msy.redwolf501.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://quw.bjfxy.top

[P03] 生成短随机字符串
来源：http://llz.vqdsnc.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tdc.shzxlz.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qwa.yuanzhike.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://grf.ppjwa.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dyf.tanke756.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yvo.jinqigfzy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://elr.cheryme.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://qsp.kuanghao11.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qnb.fengsongda.top

[P04] 求长度
来源：http://pjp.fehbvm.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nas.ybcxt.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qak.yuxming.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lmz.jlsjyb.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mee.gzhubu.top

Java: list.size();  map.size();  s.length()
来源：http://xkb.hfpthk.cn

Go:   len(arr);  len(m)
来源：http://hqb.hnxiangtu.top

Ruby: x.length;  x.size
来源：http://ymc.pycfn.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://ngi.aizwys.cn

[P05] 判断两个对象内容是否相等
来源：http://ohi.jinqigufen.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://nlq.hnqzz.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zna.gaohongyu789.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://plv.xylfe.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://yva.wangdashe.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zfs.smart0.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://xtd.aibaodan.cn

Ruby: a == b
来源：http://cgc.yj202588.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fgs.jinqigfzy.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ajs.fengsongda.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jzz.zdqjudy.top

PHP:  if (empty($x)) {}
来源：http://oei.sysykeji.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xje.sysykeji.top

TS:   if (x == null) {}
来源：http://btu.bjfxy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ijn.52xcode.cn

Go:   if x == nil {}
来源：http://ial.tanke756.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vrm.jinyuanbaomall.cn

C#:   if (x is null) {}
来源：http://rvh.chenjidiqi.icu

[P07] 防抖与节流
来源：http://rde.snrcjt.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jut.316326.xyz

PHP:  // 手写时间戳比较
来源：http://vwx.zhijiandao.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://klx.wangdashe.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wwq.yuxming.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wol.tarul.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pgk.guannengcc.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://xly.jyoumei.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zcw.xylfe.cn

[P08] 处理浮点精度问题
来源：http://xgn.316326.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://yek.jiagoushi.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bxo.yj20258.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vjq.daria6918.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lfm.gogol.net.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://siu.gzhubu.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xnf.yuxming.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fbo.sweek.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nps.zhongyouzk.top

================================================================================
来源：http://yxi.xingfuxueyuan.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dgk.birdmap.top

================================================================================
来源：http://eud.kuanghao11.cn

[Q01] 创建表
来源：http://swq.vehdjk.com

CREATE TABLE users (
来源：http://pjo.cdnleiting.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vth.sysykeji.top

name VARCHAR(50) NOT NULL,
来源：http://ndg.xuetiantiany.cn

email VARCHAR(100) UNIQUE,
来源：http://srj.pycfn.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://unu.xylfe.cn

);
来源：http://hjm.shanyushiyangtech.top

[Q02] 创建带外键的表
来源：http://mmk.zhongyouzk.top

CREATE TABLE orders (
来源：http://gnz.jinyuanbaomall.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zlh.zdqjudy.top

user_id INT NOT NULL,
来源：http://vfe.hcnkem.com

amount DECIMAL(10, 2),
来源：http://huv.zhongyouzk.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://crg.shanyushiyangtech.top

);
来源：http://bpi.bbcook.cn

[Q03] 增加列
来源：http://slh.hnxiangtu.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mqu.smart0.xyz

[Q04] 修改列类型
来源：http://qsx.svipenyu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ynp.vqdsnc.cn

[Q05] 重命名列
来源：http://njg.sysykeji.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yzs.zdbjq.cn

[Q06] 删除列
来源：http://cvc.yueranfly.top

ALTER TABLE users DROP COLUMN age;
来源：http://kwv.fktsv.cn

[Q07] 删除表
来源：http://wrc.fehbvm.com

DROP TABLE IF EXISTS orders;
来源：http://jyl.shuidangran.top

[Q08] 创建普通索引
来源：http://dps.hnxiangtu.top

CREATE INDEX idx_users_email ON users(email);
来源：http://khw.jinyuanbaomall.cn

[Q09] 创建唯一索引
来源：http://pce.xingfuxueyuan.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xal.xinyue.icu

[Q10] 插入单行
来源：http://mmt.gzhubu.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mie.ywan-chungtsiang.top

[Q11] 一次插入多行
来源：http://jdx.jqgufenzy.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xoi.jinqigfzy.top

[Q12] 插入后取自增 ID
来源：http://wjv.redwolf501.top

INSERT INTO users (name) VALUES ('C');
来源：http://ojn.smart0.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://yjk.hongshengwenyu.top

[Q13] 忽略重复插入
来源：http://ayp.hcnkem.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zdu.daria6918.cn

[Q14] 存在则更新（upsert）
来源：http://aml.jinqigfzy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jok.meibo888.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jld.xuanzx.com

[Q15] 查询全部
来源：http://ysh.hcnkem.com

SELECT * FROM users;
来源：http://qbl.ctjpmb.com

[Q16] 查询指定列
来源：http://kfa.c1oappe.top

SELECT id, name FROM users;
来源：http://izm.xingfuxueyuan.xyz

[Q17] 条件查询
来源：http://orr.hammf.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kde.quarkkingdee.top

[Q18] 模糊匹配
来源：http://efl.jyoumei.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://sez.andypj.xyz

[Q19] 范围查询
来源：http://rqe.gzhubu.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ggo.kuanghao11.cn

[Q20] IN 列表
来源：http://qhe.nanxuanxn.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vkw.dianchejie.cn

[Q21] 空值判断
来源：http://pkv.yuanzhike.top

SELECT * FROM users WHERE email IS NULL;
来源：http://laz.fanxiaobao.xyz

[Q22] 排序
来源：http://aiz.ctjpmb.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nul.nanxuanxn.top

[Q23] 分页
来源：http://jjr.svipenyu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://biw.andypj.xyz

[Q24] 去重
来源：http://rfl.gaohongyu789.top

SELECT DISTINCT city FROM users;
来源：http://nrv.cashguo.top

[Q25] 只取前 N 条
来源：http://lda.nanxinkj.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://acb.shuidangran.top

[Q26] 计数
来源：http://xay.yvedp.cn

SELECT COUNT(*) FROM users;
来源：http://tez.ppjwa.cn

[Q27] 条件计数
来源：http://kfg.cheryme.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cur.gaohongyu789.top

[Q28] 求和与平均
来源：http://ins.jiagoushi.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pwy.yongpay.top

[Q29] 最大最小值
来源：http://sxw.smart0.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://ivi.snrcjt.cn

[Q30] 分组统计
来源：http://exh.ehwqpu.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://uty.havefunace.top

[Q31] 分组后过滤
来源：http://aby.quarkkingdee.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dby.kuanghao11.cn

[Q32] 分组拼接字符串
来源：http://zeg.xuetiantiany.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ylt.shanyushiyangkeji.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ttp.yangfankeji.com

[Q33] 多列分组
来源：http://pje.haohaochexian.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://uen.shanyushiyangkeji.top

[Q34] 每组取第一条
来源：http://cax.svipenyu.cn

SELECT * FROM (
来源：http://kpf.hcnkem.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vof.haohaochexian.top

) t WHERE rn = 1;
来源：http://ywv.yj20258888.top

[Q35] 内连接
来源：http://gzh.jlsjyb.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ovw.epnwcf.com

[Q36] 左连接
来源：http://mjn.jqgufenzy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jgk.hnxiangtu.top

[Q37] 右连接
来源：http://ohb.0kj1m.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kqa.ctjpmb.com

[Q38] 全外连接（PostgreSQL）
来源：http://rea.yuxming.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wtc.ivvv.top

[Q39] 自连接（查上下级）
来源：http://sem.andypj.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://tai.hywenlv.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ecr.shanyushiyangkeji.top

[Q40] 交叉连接（笛卡尔积）
来源：http://pov.jinghuilouyu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://iaf.zycfv.cn

[Q41] 多表连接
来源：http://jol.chenlongwang.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://kfp.jqgfzy.top

JOIN users u ON u.id = o.user_id
来源：http://mjh.jinqigufen.top

JOIN products p ON p.id = o.product_id;
来源：http://jhk.aibaodan.cn

[Q42] 连接条件附加过滤
来源：http://whg.hnxiangtu.top

SELECT u.name, o.amount FROM users u
来源：http://cgu.jqgufenzy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yaj.chenzaomai.com

[Q43] 标量子查询
来源：http://ige.hcnkem.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://frm.aizwys.cn

[Q44] IN 子查询
来源：http://drj.zdqjudy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ubg.gzhubu.top

[Q45] EXISTS 判断存在
来源：http://qte.svipenyu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://suo.cdnleiting.top

[Q46] NOT EXISTS 判断不存在
来源：http://tbu.fehbvm.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pqr.yj20258888.top

[Q47] 与平均值比较
来源：http://aoe.jianghu66.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://flq.xuetiantiany.cn

[Q48] CTE 公用表表达式
来源：http://eif.shuidangran.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://oug.xingfuxueyuan.xyz

SELECT * FROM t WHERE c > 5;
来源：http://dtl.sweek.top

[Q49] 更新单行
来源：http://dza.redwolf501.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://auf.wangshuangyany.cn

[Q50] 批量更新
来源：http://oxj.cashguo.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gam.ivvv.top

[Q51] 用子查询更新
来源：http://pjr.pycfn.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jux.jinghuilouyu.cn

[Q52] 删除指定行
来源：http://ylz.jqgfzy.top

DELETE FROM users WHERE id = 10;
来源：http://nbk.havefunace.top

[Q53] 按条件删除
来源：http://twd.zhiwuduotai.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wnh.fzhhl.top

[Q54] 清空表
来源：http://wso.xylfe.cn

TRUNCATE TABLE logs;
来源：http://jxs.xuanzx.com

[Q55] 排名（并列占位）
来源：http://eur.zycfv.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fki.sxryk.cn

[Q56] 密集排名（并列不占位）
来源：http://bfe.wangshuangyany.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xun.cucudq.cn

[Q57] 行号
来源：http://xpj.zhaomingkeji.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xoo.bbcook.cn

[Q58] 累计求和
来源：http://qpu.ybcxt.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jjn.daria6918.cn

[Q59] 分组内累计
来源：http://wzf.316326.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://snm.yongpay.top

[Q60] 取上一行 / 下一行
来源：http://ebq.shanyushiyangtech.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://igq.zdqjudy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lll.guannengcc.top

[Q61] 移动平均
来源：http://ght.vehdjk.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rav.hnxiangtu.top

[Q62] 分组占比
来源：http://gwf.yuxming.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wsn.shuidangran.top


<!-- 参考信息 -->
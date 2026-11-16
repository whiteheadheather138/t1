代发 wailian999

Go:   // 手写递归
来源：http://afi.xziqi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rrd.chenlongwang.top

C#:   // 手写递归
来源：http://wni.cashguo.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cxv.iojbl.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xii.hcnkem.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gxm.svipenyu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kbu.xziqi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gqb.zycfv.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lic.dashuyun.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gwo.jinghuilouyu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://oyj.shzxlz.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rvz.pycfn.com

================================================================================
来源：http://gob.xuetiantiany.cn

O. 并发与异步
来源：http://qsf.cdnleiting.top

================================================================================
来源：http://rpv.xylfe.cn

[O01] 启动一个线程
来源：http://gjc.xingfuxueyuan.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pes.andypj.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lym.fehbvm.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hmq.zhongyouzk.top

TS:   // 同 JS
来源：http://tuo.yangfankeji.com

Java: new Thread(() -> f()).start()
来源：http://ctw.jiagoushi.top

Go:   go f()
来源：http://foz.bjfxy.top

Ruby: Thread.new { f }
来源：http://kqq.guowangkeji.top

C#:   Task.Run(() => F());
来源：http://rpp.ywan-chungtsiang.top

[O02] 使用线程池
来源：http://gnu.tian-w.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pya.pycfn.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xgc.0kj1m.cn

JS:   // worker_threads 线程池
来源：http://jdn.zdqjudy.top

TS:   // worker_threads 线程池
来源：http://eeg.kuanghao11.cn

Java: Executors.newFixedThreadPool(4)
来源：http://kry.iojbl.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dgf.tarul.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lsy.jinghuilouyu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://idc.cqqwz.cn

[O03] 加锁保护共享数据
来源：http://hwn.aibaodan.cn

Py:   with lock: shared += 1
来源：http://xxy.sweek.top

PHP:  // 用 flock() 做文件锁
来源：http://zaz.pycfn.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rfg.jianghu66.top

TS:   // 同 JS
来源：http://drq.ywan-chungtsiang.top

Java: synchronized (this) { shared++; }
来源：http://eku.zdqjudy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zeh.shzxlz.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://lwk.jyoumei.cn

C#:   lock (gate) { shared++; }
来源：http://nby.dashuyun.cn

[O04] 定义异步函数并等待
来源：http://you.jinqigufen.top

Py:   async def f():⏎    await g()
来源：http://ght.hnqzz.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://thp.gaohongyu789.top

JS:   async function f() { await g(); }
来源：http://xet.jinqigufen.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://fvx.bjfxy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pip.vqdsnc.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jft.jlsjyb.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ugb.jyoumei.cn

C#:   async Task F() { await G(); }
来源：http://bph.uphjek.com

[O05] 并发执行并等待全部完成
来源：http://nof.tianlin.xyz

Py:   asyncio.gather(*tasks)
来源：http://yku.hfpthk.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zyy.shangyingyoupin.top

JS:   await Promise.all(tasks)
来源：http://bwf.zhongyouzk.top

TS:   await Promise.all(tasks)
来源：http://rxg.ivvv.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fqa.yuanzhike.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://erw.sufxvd.cn

Ruby: threads.map(&:join)
来源：http://ecz.xinyue.icu

C#:   await Task.WhenAll(t1, t2)
来源：http://pwl.hcnkem.com

[O06] 使用进程池
来源：http://fsw.yuxming.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pgt.svipenyu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ohb.yj20258.top

JS:   // child_process / cluster 模块
来源：http://efm.hnxiangtu.top

TS:   // child_process / cluster 模块
来源：http://ulw.316326.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xoh.cqqwz.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kzx.zhixingplan.top

Ruby: // fork 块
来源：http://twc.andypj.xyz

C#:   Parallel.For
来源：http://ghr.jlsjyb.cn

================================================================================
来源：http://gxt.hnxiangtu.top

P. 常用工具函数
来源：http://qzs.bjfxy.top

================================================================================
来源：http://uvz.jinyuanbaomall.cn

[P01] 生成 UUID
来源：http://ffj.zhixingplan.top

Py:   str(uuid.uuid4())
来源：http://zmb.sjlbkw.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tza.jlsjyb.cn

JS:   crypto.randomUUID()
来源：http://gtz.hammf.cn

TS:   crypto.randomUUID()
来源：http://oio.wangdashe.top

Java: UUID.randomUUID().toString()
来源：http://gse.vehdjk.com

Go:   // 用 github.com/google/uuid
来源：http://sow.chenzaomai.com

Ruby: SecureRandom.uuid
来源：http://wby.jinqigufen.top

C#:   Guid.NewGuid().ToString()
来源：http://hjh.wangshuangyany.cn

[P02] MD5 / SHA256 摘要
来源：http://qsj.nanxuanxn.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xot.xziqi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ppi.9152youxi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bzf.zhoulong.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zzk.ywan-chungtsiang.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rhi.hnxiangtu.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wpg.snrcjt.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xnf.snrcjt.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://stc.pycfn.com

[P03] 生成短随机字符串
来源：http://ryz.wangdashe.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vwi.dashuyun.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dii.jinyuanbaomall.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qhx.jiagoushi.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fgl.shuidangran.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rxw.yuxming.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ulb.aizwys.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://sbm.hnxiangtu.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fqo.zhaomingkeji.xyz

[P04] 求长度
来源：http://haz.vqdsnc.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bpv.jinyuanbaomall.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ckn.fanxiaobao.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bzn.xingfuxueyuan.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xmd.nwbrower.top

Java: list.size();  map.size();  s.length()
来源：http://pyp.zhijiandao.cn

Go:   len(arr);  len(m)
来源：http://rnz.fktsv.cn

Ruby: x.length;  x.size
来源：http://qyw.zhongyouzk.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://hrf.yj202588.top

[P05] 判断两个对象内容是否相等
来源：http://nee.daxiang520.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://trk.daria6918.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cbt.yj20258888.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nwv.shangyingyoupin.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rms.sufxvd.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mdp.kuanghao11.cn

Go:   reflect.DeepEqual(a, b)
来源：http://kkr.xylfe.cn

Ruby: a == b
来源：http://hsw.shanyushiyangtech.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://amo.ywan-chungtsiang.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ogp.zhixingplan.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fso.feifeiyinyue.top

PHP:  if (empty($x)) {}
来源：http://evu.smart0.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://irz.wangdashe.top

TS:   if (x == null) {}
来源：http://xtq.vqdsnc.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://gze.yuanzhike.top

Go:   if x == nil {}
来源：http://wiq.shuidangran.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dfn.jinqigfzy.top

C#:   if (x is null) {}
来源：http://cmw.0kj1m.cn

[P07] 防抖与节流
来源：http://gft.chenzaomai.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dxc.kuanghao11.cn

PHP:  // 手写时间戳比较
来源：http://epu.ybcxt.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bld.pycfn.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jnu.jinyuanbaomall.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bzm.jqgfzy.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mvc.jqgufenzy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://lps.c1oappe.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bzq.shuidangran.top

[P08] 处理浮点精度问题
来源：http://tiq.jyoumei.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ckj.jiagoushi.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jfb.vehdjk.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jdx.tanke756.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kbz.guannengcc.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tir.jiagoushi.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://znc.ppjwa.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://iwv.iojbl.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xhh.ppjwa.cn

================================================================================
来源：http://sml.tanke756.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://uhq.gaohongyu789.top

================================================================================
来源：http://idl.316326.xyz

[Q01] 创建表
来源：http://kvh.vehdjk.com

CREATE TABLE users (
来源：http://mso.cashguo.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://yau.316326.xyz

name VARCHAR(50) NOT NULL,
来源：http://bvv.hcnkem.com

email VARCHAR(100) UNIQUE,
来源：http://okr.quarkkingdee.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cli.sxryk.cn

);
来源：http://rdl.tarul.cn

[Q02] 创建带外键的表
来源：http://dxh.zdbjq.cn

CREATE TABLE orders (
来源：http://atw.havefunace.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wfw.ybcxt.top

user_id INT NOT NULL,
来源：http://cer.snrcjt.cn

amount DECIMAL(10, 2),
来源：http://ezi.cdnleiting.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://myy.zhongyouzk.top

);
来源：http://hhc.aizwys.cn

[Q03] 增加列
来源：http://aew.wangdashe.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rws.yangfankeji.com

[Q04] 修改列类型
来源：http://kta.tianlin.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xba.gogol.net.cn

[Q05] 重命名列
来源：http://omj.sjlbkw.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://aij.sjlbkw.cn

[Q06] 删除列
来源：http://hyl.shuidangran.top

ALTER TABLE users DROP COLUMN age;
来源：http://ozx.shuidangran.top

[Q07] 删除表
来源：http://vug.jinqigfzy.top

DROP TABLE IF EXISTS orders;
来源：http://wun.chenzaomai.com

[Q08] 创建普通索引
来源：http://ntm.yj20258888.top

CREATE INDEX idx_users_email ON users(email);
来源：http://fho.hongshengwenyu.top

[Q09] 创建唯一索引
来源：http://xab.dianchejie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dxh.sweek.top

[Q10] 插入单行
来源：http://qom.zhengqikj.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://odw.yonumen.top

[Q11] 一次插入多行
来源：http://ujw.guowangkeji.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://soh.chenzaomai.com

[Q12] 插入后取自增 ID
来源：http://hsa.xylfe.cn

INSERT INTO users (name) VALUES ('C');
来源：http://lyq.chenjidiqi.icu

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bqs.hesvh.cn

[Q13] 忽略重复插入
来源：http://sll.cheryme.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://sry.nwbrower.top

[Q14] 存在则更新（upsert）
来源：http://hff.daxiang520.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bwj.yangfankeji.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yry.smart0.xyz

[Q15] 查询全部
来源：http://thv.jinqigufen.top

SELECT * FROM users;
来源：http://rnw.gzhubu.top

[Q16] 查询指定列
来源：http://yrw.sufxvd.cn

SELECT id, name FROM users;
来源：http://ghg.bbcook.cn

[Q17] 条件查询
来源：http://dud.zycfv.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://myx.yongpay.top

[Q18] 模糊匹配
来源：http://gwf.vqdsnc.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://shf.xinyue.icu

[Q19] 范围查询
来源：http://nto.pycfn.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ckb.dianchejie.cn

[Q20] IN 列表
来源：http://hzi.vehdjk.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wxn.feifeiyinyue.top

[Q21] 空值判断
来源：http://hzk.xuanzx.com

SELECT * FROM users WHERE email IS NULL;
来源：http://btm.yonumen.top

[Q22] 排序
来源：http://dpg.zhengqikj.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ont.xylfe.cn

[Q23] 分页
来源：http://vky.yangfankeji.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rrn.jlsjyb.cn

[Q24] 去重
来源：http://qup.aibaodan.cn

SELECT DISTINCT city FROM users;
来源：http://dvr.ydzc1.top

[Q25] 只取前 N 条
来源：http://guq.yj202588.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cfq.shangyingyoupin.top

[Q26] 计数
来源：http://bep.ybcxt.top

SELECT COUNT(*) FROM users;
来源：http://itt.zdbjq.cn

[Q27] 条件计数
来源：http://xpc.yj20258.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kco.c1oappe.top

[Q28] 求和与平均
来源：http://tzr.sufxvd.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://brh.xuetiantiany.cn

[Q29] 最大最小值
来源：http://bhf.9152youxi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://czc.hfpthk.cn

[Q30] 分组统计
来源：http://zxh.fehbvm.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://anm.yanxiufei.cn

[Q31] 分组后过滤
来源：http://ozb.meibo888.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fdd.xylfe.cn

[Q32] 分组拼接字符串
来源：http://uiu.jlsjyb.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://teg.yfazqb.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mli.yuanzhike.top

[Q33] 多列分组
来源：http://ysm.nanxinkj.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lwr.shzxlz.cn

[Q34] 每组取第一条
来源：http://cky.iojbl.cn

SELECT * FROM (
来源：http://lhj.cheryme.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qll.zhoulong.xyz

) t WHERE rn = 1;
来源：http://dlp.jinyuanbaomall.cn

[Q35] 内连接
来源：http://atv.shzxlz.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://azy.jlsjyb.cn

[Q36] 左连接
来源：http://wce.zhaomingkeji.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fro.guannengcc.top

[Q37] 右连接
来源：http://tpr.zhiwuduotai.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lom.jinqigfzy.top

[Q38] 全外连接（PostgreSQL）
来源：http://jey.sxryk.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wsp.xylfe.cn

[Q39] 自连接（查上下级）
来源：http://gpg.cashguo.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://anu.wangdashe.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nuf.jlsjyb.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://bij.snrcjt.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://yrv.shangyingyoupin.top

[Q41] 多表连接
来源：http://wdc.yangfankeji.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://jxe.ydzc1.top

JOIN users u ON u.id = o.user_id
来源：http://fky.meibo888.top

JOIN products p ON p.id = o.product_id;
来源：http://fcn.aibaodan.cn

[Q42] 连接条件附加过滤
来源：http://iiy.ppjwa.cn

SELECT u.name, o.amount FROM users u
来源：http://flb.zycfv.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mbn.iojbl.cn

[Q43] 标量子查询
来源：http://jjg.dashuyun.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rte.yvedp.cn

[Q44] IN 子查询
来源：http://ohw.zhongyouzk.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vsh.yonumen.top

[Q45] EXISTS 判断存在
来源：http://iej.jinqigfzy.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cop.zhixingplan.top

[Q46] NOT EXISTS 判断不存在
来源：http://tuy.fanxiaobao.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bdj.nanxuanxn.top

[Q47] 与平均值比较
来源：http://ykl.feifeiyinyue.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wsp.birdmap.top

[Q48] CTE 公用表表达式
来源：http://ycs.cdnleiting.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bmk.sjlbkw.cn

SELECT * FROM t WHERE c > 5;
来源：http://wyv.ybcxt.top

[Q49] 更新单行
来源：http://mgv.zhaomingkeji.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cie.fehbvm.com

[Q50] 批量更新
来源：http://qqw.shanyushiyangtech.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xgr.9152youxi.cn

[Q51] 用子查询更新
来源：http://bah.dianchejie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zpn.jinyuanbaomall.cn

[Q52] 删除指定行
来源：http://jmr.pycfn.com

DELETE FROM users WHERE id = 10;
来源：http://pti.redwolf501.top

[Q53] 按条件删除
来源：http://kpt.zdqjudy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://maz.fehbvm.com

[Q54] 清空表
来源：http://ukb.hesvh.cn

TRUNCATE TABLE logs;
来源：http://tun.hammf.cn

[Q55] 排名（并列占位）
来源：http://tfc.jyoumei.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rrv.havefunace.top

[Q56] 密集排名（并列不占位）
来源：http://apw.hnqzz.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jwx.yj202588.top

[Q57] 行号
来源：http://uxx.hcnkem.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://inl.gzhubu.top

[Q58] 累计求和
来源：http://gqk.jqgufenzy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zmh.hywenlv.cn

[Q59] 分组内累计
来源：http://wof.fzhhl.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cvn.shanyushiyangkeji.top

[Q60] 取上一行 / 下一行
来源：http://dlq.feifeiyinyue.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://swk.mhx1999.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zhu.vehdjk.com

[Q61] 移动平均
来源：http://ckk.zhaomingkeji.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lkf.nanxinkj.top

[Q62] 分组占比
来源：http://uay.pengpengdd.cyou

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rhn.mhx1999.top

[Q63] 开启事务
来源：http://dvm.jlsjyb.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ltc.aizwys.cn

[Q64] 提交事务
来源：http://bns.meibo888.top

COMMIT;
来源：http://fax.zhaomingkeji.xyz

[Q65] 回滚事务
来源：http://doz.dianchejie.cn

ROLLBACK;
来源：http://dnb.hywenlv.cn

[Q66] 行锁查询
来源：http://pon.0kj1m.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bsv.jianghu66.top


<!-- 参考信息 -->
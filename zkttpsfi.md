代发 wailian999

================================================================================
来源：http://byk.sysykeji.top

O. 并发与异步
来源：http://bjb.pengpengdd.cyou

================================================================================
来源：http://vgv.meibo888.top

[O01] 启动一个线程
来源：http://elj.pycfn.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zre.yuanzhike.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kcj.xuetiantiany.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tlz.jianghu66.top

TS:   // 同 JS
来源：http://psz.cashguo.top

Java: new Thread(() -> f()).start()
来源：http://mcd.tianlin.xyz

Go:   go f()
来源：http://uwi.yonumen.top

Ruby: Thread.new { f }
来源：http://mzy.chenjidiqi.icu

C#:   Task.Run(() => F());
来源：http://zfx.redwolf501.top

[O02] 使用线程池
来源：http://qzc.tanke756.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nzw.hysaishi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ahw.jiagoushi.top

JS:   // worker_threads 线程池
来源：http://koe.bjfxy.top

TS:   // worker_threads 线程池
来源：http://olh.andypj.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://egt.jqgufenzy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ccu.hysaishi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lbb.tian-w.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gwe.uphjek.com

[O03] 加锁保护共享数据
来源：http://yoe.yangfankeji.com

Py:   with lock: shared += 1
来源：http://nqd.fzhhl.top

PHP:  // 用 flock() 做文件锁
来源：http://sex.jianghu66.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ixc.zhiwuduotai.top

TS:   // 同 JS
来源：http://lrt.vqdsnc.cn

Java: synchronized (this) { shared++; }
来源：http://kxh.vehdjk.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hon.xingfuxueyuan.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://gem.cqqwz.cn

C#:   lock (gate) { shared++; }
来源：http://ers.xuanzx.com

[O04] 定义异步函数并等待
来源：http://jod.bjfxy.top

Py:   async def f():⏎    await g()
来源：http://uiz.daxiang520.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://txz.nanxuanxn.top

JS:   async function f() { await g(); }
来源：http://lrh.zhaomingkeji.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://jqw.tian-w.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://oiu.fehbvm.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xaj.zycfv.cn

Ruby: # 用 Fiber 或 async gem
来源：http://xae.ybcxt.top

C#:   async Task F() { await G(); }
来源：http://wyy.ctjpmb.com

[O05] 并发执行并等待全部完成
来源：http://qbs.zhongyouzk.top

Py:   asyncio.gather(*tasks)
来源：http://sxu.bbcook.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xiz.yongpay.top

JS:   await Promise.all(tasks)
来源：http://xtm.tianlin.xyz

TS:   await Promise.all(tasks)
来源：http://vsf.cqqwz.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dqb.xuetiantiany.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://khb.yj20258.top

Ruby: threads.map(&:join)
来源：http://ygk.dashuyun.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://lwj.hfpthk.cn

[O06] 使用进程池
来源：http://hbr.feifeiyinyue.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gle.vqdsnc.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://jie.ydzc1.top

JS:   // child_process / cluster 模块
来源：http://ziu.tian-w.cn

TS:   // child_process / cluster 模块
来源：http://uuf.daxiang520.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vip.snrcjt.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dyn.bbcook.cn

Ruby: // fork 块
来源：http://tkq.ivvv.top

C#:   Parallel.For
来源：http://axo.shangyingyoupin.top

================================================================================
来源：http://jin.zhaomingkeji.xyz

P. 常用工具函数
来源：http://hdj.svipenyu.cn

================================================================================
来源：http://iws.jyoumei.cn

[P01] 生成 UUID
来源：http://xoo.andypj.xyz

Py:   str(uuid.uuid4())
来源：http://wjw.shanyushiyangkeji.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fjf.mhx1999.top

JS:   crypto.randomUUID()
来源：http://jev.jinghuilouyu.cn

TS:   crypto.randomUUID()
来源：http://yfk.ybcxt.top

Java: UUID.randomUUID().toString()
来源：http://jzm.pengpengdd.cyou

Go:   // 用 github.com/google/uuid
来源：http://gaq.snrcjt.cn

Ruby: SecureRandom.uuid
来源：http://lns.daxiang520.top

C#:   Guid.NewGuid().ToString()
来源：http://qsj.wangdashe.top

[P02] MD5 / SHA256 摘要
来源：http://ucc.hnqzz.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ccs.jyoumei.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://qch.sufxvd.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lmw.daria6918.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tic.svipenyu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ubj.hnxiangtu.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://guf.hongshengwenyu.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pfv.mhx1999.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nya.yuxming.cn

[P03] 生成短随机字符串
来源：http://oui.cqqwz.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yuz.tanke756.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qhc.daria6918.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rkj.aibaodan.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ksb.tarul.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rnn.yfazqb.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://psl.jinghuilouyu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://cgs.jinyuanbaomall.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zxg.52xcode.cn

[P04] 求长度
来源：http://aao.yj202588.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uzk.xuanzx.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://axf.yueranfly.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://evt.fzhhl.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tqu.chenlongwang.top

Java: list.size();  map.size();  s.length()
来源：http://yhy.dianchejie.cn

Go:   len(arr);  len(m)
来源：http://byp.wangshuangyany.cn

Ruby: x.length;  x.size
来源：http://oqy.fanxiaobao.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://pwg.iojbl.cn

[P05] 判断两个对象内容是否相等
来源：http://syd.fengsongda.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://nan.sufxvd.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dbl.uphjek.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hsm.tanke756.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vxp.cqqwz.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://sbf.cheryme.top

Go:   reflect.DeepEqual(a, b)
来源：http://spa.hysaishi.cn

Ruby: a == b
来源：http://rvu.xuanzx.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lbk.feifeiyinyue.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hau.wangdashe.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tqe.nanxinkj.top

PHP:  if (empty($x)) {}
来源：http://zxz.xziqi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://uea.smart0.xyz

TS:   if (x == null) {}
来源：http://vsi.uphjek.com

Java: if (x == null || x.isEmpty()) {}
来源：http://xus.guowangkeji.top

Go:   if x == nil {}
来源：http://bsz.vqdsnc.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ajr.jianghu66.top

C#:   if (x is null) {}
来源：http://eal.jianghu66.top

[P07] 防抖与节流
来源：http://dyt.hesvh.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lzk.redwolf501.top

PHP:  // 手写时间戳比较
来源：http://lew.yuanzhike.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://atk.zhoulong.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ssu.fehbvm.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ocw.hongshengwenyu.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://stv.0kj1m.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://wct.xingfuxueyuan.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xsn.yuxming.cn

[P08] 处理浮点精度问题
来源：http://fen.yongpay.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://nay.andypj.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kyu.fktsv.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://sga.pycfn.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bln.xuetiantiany.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wml.haohaochexian.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://odp.c1oappe.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wfm.hfpthk.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qde.ydzc1.top

================================================================================
来源：http://xvy.cheryme.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tfy.316326.xyz

================================================================================
来源：http://dus.c1oappe.top

[Q01] 创建表
来源：http://owp.yfazqb.com

CREATE TABLE users (
来源：http://xyu.sjlbkw.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mss.chenzaomai.com

name VARCHAR(50) NOT NULL,
来源：http://kgr.52xcode.cn

email VARCHAR(100) UNIQUE,
来源：http://gzx.yj20258888.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://oqk.guowangkeji.top

);
来源：http://egr.yvedp.cn

[Q02] 创建带外键的表
来源：http://tfm.cucudq.cn

CREATE TABLE orders (
来源：http://xgq.xinyue.icu

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kdb.cqqwz.cn

user_id INT NOT NULL,
来源：http://otj.cheryme.top

amount DECIMAL(10, 2),
来源：http://xhw.mhx1999.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mvj.kuanghao11.cn

);
来源：http://jjq.ehwqpu.com

[Q03] 增加列
来源：http://qpd.havefunace.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kqk.guowangkeji.top

[Q04] 修改列类型
来源：http://ehc.shzxlz.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lhr.cashguo.top

[Q05] 重命名列
来源：http://fjo.hysaishi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ync.fehbvm.com

[Q06] 删除列
来源：http://mos.ppjwa.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ceu.sxryk.cn

[Q07] 删除表
来源：http://ciw.yj202588.top

DROP TABLE IF EXISTS orders;
来源：http://obi.yuxming.cn

[Q08] 创建普通索引
来源：http://upn.zdqjudy.top

CREATE INDEX idx_users_email ON users(email);
来源：http://yei.nanxuanxn.top

[Q09] 创建唯一索引
来源：http://qlg.vehdjk.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://edo.birdmap.top

[Q10] 插入单行
来源：http://suu.hammf.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mlw.gogol.net.cn

[Q11] 一次插入多行
来源：http://uvg.ivvv.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://osl.bbcook.cn

[Q12] 插入后取自增 ID
来源：http://ucj.nanxinkj.top

INSERT INTO users (name) VALUES ('C');
来源：http://gak.zhixingplan.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://usq.vqdsnc.cn

[Q13] 忽略重复插入
来源：http://uyp.zhaomingkeji.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bja.tarul.cn

[Q14] 存在则更新（upsert）
来源：http://ctk.tianlin.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dwm.ywan-chungtsiang.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pem.zhaomingkeji.xyz

[Q15] 查询全部
来源：http://fao.zhoulong.xyz

SELECT * FROM users;
来源：http://sfz.zhaomingkeji.xyz

[Q16] 查询指定列
来源：http://bao.gogol.net.cn

SELECT id, name FROM users;
来源：http://fhv.gzhubu.top

[Q17] 条件查询
来源：http://lgb.chenjidiqi.icu

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xct.shanyushiyangkeji.top

[Q18] 模糊匹配
来源：http://kjb.chenzaomai.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ewu.jinghuilouyu.cn

[Q19] 范围查询
来源：http://osk.jlsjyb.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://uet.zhaomingkeji.xyz

[Q20] IN 列表
来源：http://jlj.ybcxt.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wsh.guannengcc.top

[Q21] 空值判断
来源：http://wpl.ywan-chungtsiang.top

SELECT * FROM users WHERE email IS NULL;
来源：http://yit.yongpay.top

[Q22] 排序
来源：http://snp.bjfxy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mww.jinyuanbaomall.cn

[Q23] 分页
来源：http://dyf.zhixingplan.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://cim.daria6918.cn

[Q24] 去重
来源：http://xsv.gzhubu.top

SELECT DISTINCT city FROM users;
来源：http://dmo.yangfankeji.com

[Q25] 只取前 N 条
来源：http://uyx.zhaomingkeji.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bam.ydjk.org.cn

[Q26] 计数
来源：http://ptz.sufxvd.cn

SELECT COUNT(*) FROM users;
来源：http://wig.birdmap.top

[Q27] 条件计数
来源：http://vok.fengsongda.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ucl.gogol.net.cn

[Q28] 求和与平均
来源：http://oqq.zycfv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://doc.shangyingyoupin.top

[Q29] 最大最小值
来源：http://dfb.zdbjq.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://hum.jyoumei.cn

[Q30] 分组统计
来源：http://tel.jlsjyb.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wcn.jianghu66.top

[Q31] 分组后过滤
来源：http://etp.shangyingyoupin.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://npd.daxiang520.top

[Q32] 分组拼接字符串
来源：http://jbq.fanxiaobao.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://uka.jinqigufen.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qru.gogol.net.cn

[Q33] 多列分组
来源：http://iov.haohaochexian.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ncq.jinghuilouyu.cn

[Q34] 每组取第一条
来源：http://aoy.wangdashe.top

SELECT * FROM (
来源：http://emk.svipenyu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qet.bbcook.cn

) t WHERE rn = 1;
来源：http://cit.cheryme.top

[Q35] 内连接
来源：http://xmb.daxiang520.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rjl.wangshuangyany.cn

[Q36] 左连接
来源：http://ymz.zhaomingkeji.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cxr.wangshuangyany.cn

[Q37] 右连接
来源：http://ozr.fengsongda.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gct.bbcook.cn

[Q38] 全外连接（PostgreSQL）
来源：http://eud.zhiwuduotai.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hgu.yueranfly.top

[Q39] 自连接（查上下级）
来源：http://uba.ehwqpu.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://kan.guannengcc.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://duq.quarkkingdee.top

[Q40] 交叉连接（笛卡尔积）
来源：http://bwd.cucudq.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bbi.yvedp.cn

[Q41] 多表连接
来源：http://jgm.9152youxi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://nsz.jyoumei.cn

JOIN users u ON u.id = o.user_id
来源：http://twu.xinyue.icu

JOIN products p ON p.id = o.product_id;
来源：http://kkz.tianlin.xyz

[Q42] 连接条件附加过滤
来源：http://kxc.sxryk.cn

SELECT u.name, o.amount FROM users u
来源：http://abt.daria6918.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wsc.gaohongyu789.top

[Q43] 标量子查询
来源：http://bvx.quarkkingdee.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bji.redwolf501.top

[Q44] IN 子查询
来源：http://jiz.nanxinkj.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lli.sjlbkw.cn

[Q45] EXISTS 判断存在
来源：http://onl.chenlongwang.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bvc.bbcook.cn

[Q46] NOT EXISTS 判断不存在
来源：http://fhj.tian-w.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://idi.xuetiantiany.cn

[Q47] 与平均值比较
来源：http://dbi.gzhubu.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ibb.ehwqpu.com

[Q48] CTE 公用表表达式
来源：http://ehw.52xcode.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xmb.zhaomingkeji.xyz

SELECT * FROM t WHERE c > 5;
来源：http://cxk.fzhhl.top

[Q49] 更新单行
来源：http://oki.nanxuanxn.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ibf.jianghu66.top

[Q50] 批量更新
来源：http://trc.daria6918.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rny.ybcxt.top

[Q51] 用子查询更新
来源：http://fke.ywan-chungtsiang.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://eyl.yongpay.top

[Q52] 删除指定行
来源：http://tbr.kuanghao11.cn

DELETE FROM users WHERE id = 10;
来源：http://pzo.zhixingplan.top

[Q53] 按条件删除
来源：http://jdc.sxryk.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fee.svipenyu.cn

[Q54] 清空表
来源：http://fex.yj20258.top

TRUNCATE TABLE logs;
来源：http://gzy.mhx1999.top

[Q55] 排名（并列占位）
来源：http://gxf.dashuyun.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qth.gotoacloud.top

[Q56] 密集排名（并列不占位）
来源：http://khw.gaohongyu789.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://enl.ivvv.top

[Q57] 行号
来源：http://buj.ydzc1.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://uds.tanke756.top

[Q58] 累计求和
来源：http://atl.feifeiyinyue.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ymp.fengsongda.top

[Q59] 分组内累计
来源：http://puy.xinyue.icu

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cbq.fengsongda.top

[Q60] 取上一行 / 下一行
来源：http://zmw.birdmap.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ksj.yvedp.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baz.epnwcf.com

[Q61] 移动平均
来源：http://xjc.zhaomingkeji.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://orj.gogol.net.cn

[Q62] 分组占比
来源：http://caa.ywan-chungtsiang.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tbv.jiagoushi.top

[Q63] 开启事务
来源：http://qpr.hywenlv.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://czn.cdnleiting.top

[Q64] 提交事务
来源：http://vzh.gogol.net.cn

COMMIT;
来源：http://spx.yueranfly.top

[Q65] 回滚事务
来源：http://zor.guannengcc.top

ROLLBACK;
来源：http://oep.9152youxi.cn

[Q66] 行锁查询
来源：http://ddh.tanke756.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hdf.cashguo.top

[Q67] 设置隔离级别
来源：http://vvn.tianlin.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lvh.hysaishi.cn

[Q68] 保存点
来源：http://qsq.xuanzx.com

SAVEPOINT sp1;
来源：http://rmw.hcnkem.com

ROLLBACK TO sp1;
来源：http://qkm.xuetiantiany.cn

[Q69] 查看执行计划
来源：http://mhf.hywenlv.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cid.meibo888.top

[Q70] 更新统计信息
来源：http://xwi.cashguo.top

ANALYZE TABLE users;
来源：http://twt.hammf.cn

[Q71] 查看建表语句
来源：http://dbe.xuanzx.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ozq.hnqzz.top

[Q72] 查看索引
来源：http://wtd.xylfe.cn


<!-- 参考信息 -->
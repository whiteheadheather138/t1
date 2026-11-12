代发 wailian999

TS:   // worker_threads 线程池
来源：http://wxh.yangfankeji.com

Java: Executors.newFixedThreadPool(4)
来源：http://bmr.tianlin.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://inh.yongpay.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://llr.ehwqpu.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pbz.hfpthk.cn

[O03] 加锁保护共享数据
来源：http://bnn.vehdjk.com

Py:   with lock: shared += 1
来源：http://vux.zhixingplan.top

PHP:  // 用 flock() 做文件锁
来源：http://twg.fktsv.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lsq.zhengqikj.top

TS:   // 同 JS
来源：http://squ.yangfankeji.com

Java: synchronized (this) { shared++; }
来源：http://dfu.316326.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gev.yangfankeji.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://rht.xuetiantiany.cn

C#:   lock (gate) { shared++; }
来源：http://ckk.sjlbkw.cn

[O04] 定义异步函数并等待
来源：http://sed.zhiwuduotai.top

Py:   async def f():⏎    await g()
来源：http://mir.smart0.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yyf.birdmap.top

JS:   async function f() { await g(); }
来源：http://pse.xziqi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://kuj.fktsv.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rca.yuanzhike.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vsy.zhiwuduotai.top

Ruby: # 用 Fiber 或 async gem
来源：http://grt.zhengqikj.top

C#:   async Task F() { await G(); }
来源：http://lmd.gotoacloud.top

[O05] 并发执行并等待全部完成
来源：http://ijm.haohaochexian.top

Py:   asyncio.gather(*tasks)
来源：http://nwt.cheryme.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://poj.ywan-chungtsiang.top

JS:   await Promise.all(tasks)
来源：http://xpf.jinqigfzy.top

TS:   await Promise.all(tasks)
来源：http://bcw.chenjidiqi.icu

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vks.jqgfzy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qge.c1oappe.top

Ruby: threads.map(&:join)
来源：http://evj.zhengqikj.top

C#:   await Task.WhenAll(t1, t2)
来源：http://zfn.redwolf501.top

[O06] 使用进程池
来源：http://ocx.zhixingplan.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://iej.feifeiyinyue.top

PHP:  // pcntl_fork 或多进程队列
来源：http://wvw.yuxming.cn

JS:   // child_process / cluster 模块
来源：http://zng.sxryk.cn

TS:   // child_process / cluster 模块
来源：http://lli.nwbrower.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ptg.yj202588.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nle.mhx1999.top

Ruby: // fork 块
来源：http://smt.zhijiandao.cn

C#:   Parallel.For
来源：http://fte.shzxlz.cn

================================================================================
来源：http://hrq.yvedp.cn

P. 常用工具函数
来源：http://sbp.hnxiangtu.top

================================================================================
来源：http://dzu.jinqigufen.top

[P01] 生成 UUID
来源：http://her.0kj1m.cn

Py:   str(uuid.uuid4())
来源：http://vnm.feifeiyinyue.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lyh.cdnleiting.top

JS:   crypto.randomUUID()
来源：http://mma.yj20258888.top

TS:   crypto.randomUUID()
来源：http://eph.quarkkingdee.top

Java: UUID.randomUUID().toString()
来源：http://daz.ctjpmb.com

Go:   // 用 github.com/google/uuid
来源：http://hvu.pycfn.com

Ruby: SecureRandom.uuid
来源：http://kuw.jiagoushi.top

C#:   Guid.NewGuid().ToString()
来源：http://vof.yj20258888.top

[P02] MD5 / SHA256 摘要
来源：http://iok.jyoumei.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hwk.jinghuilouyu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ojr.ppjwa.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cyt.hammf.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yzb.zdbjq.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://myi.smart0.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ihw.dianchejie.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nzh.yonumen.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ags.chenzaomai.com

[P03] 生成短随机字符串
来源：http://wmo.bbcook.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rqh.andypj.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://skw.jlsjyb.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jfw.uphjek.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nyr.tianlin.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://his.shangyingyoupin.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://frp.jyoumei.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://cko.jiagoushi.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://waa.tarul.cn

[P04] 求长度
来源：http://kbp.jqgfzy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jgw.zdbjq.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://omp.xinyue.icu

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mmc.yj20258.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://glg.jinqigfzy.top

Java: list.size();  map.size();  s.length()
来源：http://fdv.ctjpmb.com

Go:   len(arr);  len(m)
来源：http://khq.xylfe.cn

Ruby: x.length;  x.size
来源：http://gez.guowangkeji.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://dfe.yueranfly.top

[P05] 判断两个对象内容是否相等
来源：http://rmf.zhaomingkeji.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://wzh.yueranfly.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://eeg.wangdashe.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fsb.ehwqpu.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bpa.gzhubu.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://coj.ydzc1.top

Go:   reflect.DeepEqual(a, b)
来源：http://fst.hcnkem.com

Ruby: a == b
来源：http://guu.hnqzz.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://imw.ydzc1.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zwj.zhoulong.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ylm.hywenlv.cn

PHP:  if (empty($x)) {}
来源：http://bng.dashuyun.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xnl.jinqigfzy.top

TS:   if (x == null) {}
来源：http://dng.jyoumei.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://mmh.ehwqpu.com

Go:   if x == nil {}
来源：http://kru.aibaodan.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kte.havefunace.top

C#:   if (x is null) {}
来源：http://lwo.fanxiaobao.xyz

[P07] 防抖与节流
来源：http://lqt.hfpthk.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hky.zdqjudy.top

PHP:  // 手写时间戳比较
来源：http://xhv.dashuyun.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jan.jinyuanbaomall.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gvq.jlsjyb.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hvi.jiagoushi.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rmb.gaohongyu789.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://dzg.sufxvd.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kff.havefunace.top

[P08] 处理浮点精度问题
来源：http://gxy.quarkkingdee.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://tui.xylfe.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://imz.zhiwuduotai.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://oph.jiagoushi.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gee.iojbl.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mel.yj20258888.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dgf.ehwqpu.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fra.shzxlz.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://yvq.vehdjk.com

================================================================================
来源：http://sag.hywenlv.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qgn.sweek.top

================================================================================
来源：http://dqn.yangfankeji.com

[Q01] 创建表
来源：http://fcr.meibo888.top

CREATE TABLE users (
来源：http://twz.52xcode.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://odm.fanxiaobao.xyz

name VARCHAR(50) NOT NULL,
来源：http://jrm.jinqigufen.top

email VARCHAR(100) UNIQUE,
来源：http://ior.jyoumei.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gsc.hcnkem.com

);
来源：http://ndn.ehwqpu.com

[Q02] 创建带外键的表
来源：http://sat.jqgufenzy.top

CREATE TABLE orders (
来源：http://koz.ehwqpu.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ggx.meibo888.top

user_id INT NOT NULL,
来源：http://dww.yj20258.top

amount DECIMAL(10, 2),
来源：http://ope.jianghu66.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zoc.fanxiaobao.xyz

);
来源：http://vap.jqgfzy.top

[Q03] 增加列
来源：http://uuu.zdqjudy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://csr.sxryk.cn

[Q04] 修改列类型
来源：http://gmj.zdqjudy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jzz.ywan-chungtsiang.top

[Q05] 重命名列
来源：http://xru.yanxiufei.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://axf.chenjidiqi.icu

[Q06] 删除列
来源：http://skc.wangshuangyany.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ari.zhoulong.xyz

[Q07] 删除表
来源：http://qit.ctjpmb.com

DROP TABLE IF EXISTS orders;
来源：http://pov.yonumen.top

[Q08] 创建普通索引
来源：http://zep.pengpengdd.cyou

CREATE INDEX idx_users_email ON users(email);
来源：http://jrf.yj202588.top

[Q09] 创建唯一索引
来源：http://wjc.yj20258888.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wfm.yj20258888.top

[Q10] 插入单行
来源：http://mgw.zycfv.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fjo.dianchejie.cn

[Q11] 一次插入多行
来源：http://ajt.quarkkingdee.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lkn.snrcjt.cn

[Q12] 插入后取自增 ID
来源：http://zgr.pengpengdd.cyou

INSERT INTO users (name) VALUES ('C');
来源：http://yeg.hongshengwenyu.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hbw.ydjk.org.cn

[Q13] 忽略重复插入
来源：http://tzr.bjfxy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jhg.52xcode.cn

[Q14] 存在则更新（upsert）
来源：http://roh.chenzaomai.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wwq.52xcode.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xec.uphjek.com

[Q15] 查询全部
来源：http://yha.9152youxi.cn

SELECT * FROM users;
来源：http://zzn.jqgfzy.top

[Q16] 查询指定列
来源：http://hsd.ydjk.org.cn

SELECT id, name FROM users;
来源：http://yyp.hcnkem.com

[Q17] 条件查询
来源：http://tsm.shanyushiyangtech.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zjr.wangdashe.top

[Q18] 模糊匹配
来源：http://fot.zhiwuduotai.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://frk.ydzc1.top

[Q19] 范围查询
来源：http://ava.cheryme.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://voe.yonumen.top

[Q20] IN 列表
来源：http://quo.fengsongda.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fxv.quarkkingdee.top

[Q21] 空值判断
来源：http://kvg.pengpengdd.cyou

SELECT * FROM users WHERE email IS NULL;
来源：http://ozh.havefunace.top

[Q22] 排序
来源：http://vbm.xuanzx.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kuj.dianchejie.cn

[Q23] 分页
来源：http://qsp.vqdsnc.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bvs.xingfuxueyuan.xyz

[Q24] 去重
来源：http://hix.nwbrower.top

SELECT DISTINCT city FROM users;
来源：http://twx.wangshuangyany.cn

[Q25] 只取前 N 条
来源：http://kwz.zhaomingkeji.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qws.xinyue.icu

[Q26] 计数
来源：http://xdh.ywan-chungtsiang.top

SELECT COUNT(*) FROM users;
来源：http://vek.cqqwz.cn

[Q27] 条件计数
来源：http://ptu.guannengcc.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nvk.yj20258.top

[Q28] 求和与平均
来源：http://zeu.cashguo.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fde.sufxvd.cn

[Q29] 最大最小值
来源：http://yiu.jinghuilouyu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://isd.yanxiufei.cn

[Q30] 分组统计
来源：http://woz.andypj.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ssy.kuanghao11.cn

[Q31] 分组后过滤
来源：http://qfy.hongshengwenyu.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://niv.sufxvd.cn

[Q32] 分组拼接字符串
来源：http://nqd.hongshengwenyu.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rvn.jinghuilouyu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qhh.fzhhl.top

[Q33] 多列分组
来源：http://gwl.sxryk.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hrg.jlsjyb.cn

[Q34] 每组取第一条
来源：http://gmc.zhijiandao.cn

SELECT * FROM (
来源：http://wye.feifeiyinyue.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ugt.zdbjq.cn

) t WHERE rn = 1;
来源：http://uun.smart0.xyz

[Q35] 内连接
来源：http://otv.xinyue.icu

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xok.kuanghao11.cn

[Q36] 左连接
来源：http://bbi.pengpengdd.cyou

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jzn.snrcjt.cn

[Q37] 右连接
来源：http://okh.cdnleiting.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jno.zhengqikj.top

[Q38] 全外连接（PostgreSQL）
来源：http://zmp.fengsongda.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://daf.nanxuanxn.top

[Q39] 自连接（查上下级）
来源：http://qii.yvedp.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://kkl.meibo888.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dsd.yj20258888.top

[Q40] 交叉连接（笛卡尔积）
来源：http://nmx.jqgufenzy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qzr.yj20258.top

[Q41] 多表连接
来源：http://mrw.sjlbkw.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://lee.mhx1999.top

JOIN users u ON u.id = o.user_id
来源：http://kup.fktsv.cn

JOIN products p ON p.id = o.product_id;
来源：http://bdh.yangfankeji.com

[Q42] 连接条件附加过滤
来源：http://vec.fehbvm.com

SELECT u.name, o.amount FROM users u
来源：http://ahu.aibaodan.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://cbs.gogol.net.cn

[Q43] 标量子查询
来源：http://swy.xziqi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vew.xylfe.cn

[Q44] IN 子查询
来源：http://glr.epnwcf.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://okf.zhengqikj.top

[Q45] EXISTS 判断存在
来源：http://stc.hesvh.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ril.hcnkem.com

[Q46] NOT EXISTS 判断不存在
来源：http://pcc.havefunace.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bgb.snrcjt.cn

[Q47] 与平均值比较
来源：http://dxa.smart0.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://atl.zdbjq.cn

[Q48] CTE 公用表表达式
来源：http://eqj.zhixingplan.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mxv.xylfe.cn

SELECT * FROM t WHERE c > 5;
来源：http://jcm.sxryk.cn

[Q49] 更新单行
来源：http://nmg.yj20258888.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://thd.chenjidiqi.icu

[Q50] 批量更新
来源：http://mbe.jlsjyb.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ppd.uphjek.com

[Q51] 用子查询更新
来源：http://dpl.pengpengdd.cyou

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gli.zhaomingkeji.xyz

[Q52] 删除指定行
来源：http://beh.yueranfly.top

DELETE FROM users WHERE id = 10;
来源：http://kdm.gzhubu.top

[Q53] 按条件删除
来源：http://hrx.tian-w.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://cuh.cqqwz.cn

[Q54] 清空表
来源：http://ilh.mhx1999.top

TRUNCATE TABLE logs;
来源：http://qns.zhoulong.xyz

[Q55] 排名（并列占位）
来源：http://tzp.xziqi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://uen.fktsv.cn

[Q56] 密集排名（并列不占位）
来源：http://lui.ydzc1.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://cci.zhoulong.xyz

[Q57] 行号
来源：http://lxo.tian-w.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wzb.zhijiandao.cn

[Q58] 累计求和
来源：http://dzr.sxryk.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gqa.hnqzz.top

[Q59] 分组内累计
来源：http://qjx.svipenyu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://daf.gogol.net.cn

[Q60] 取上一行 / 下一行
来源：http://red.sweek.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://egk.yongpay.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zru.quarkkingdee.top

[Q61] 移动平均
来源：http://dvi.ybcxt.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qjk.nanxinkj.top

[Q62] 分组占比
来源：http://bla.yj20258888.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kwu.52xcode.cn

[Q63] 开启事务
来源：http://ggy.ppjwa.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://eut.zycfv.cn

[Q64] 提交事务
来源：http://wcc.nanxuanxn.top

COMMIT;
来源：http://opz.zdbjq.cn

[Q65] 回滚事务
来源：http://uiv.sufxvd.cn

ROLLBACK;
来源：http://drj.nanxuanxn.top

[Q66] 行锁查询
来源：http://bki.meibo888.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://iza.jiagoushi.top

[Q67] 设置隔离级别
来源：http://pah.smart0.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jio.yfazqb.com

[Q68] 保存点
来源：http://xjs.0kj1m.cn

SAVEPOINT sp1;
来源：http://cmm.meibo888.top

ROLLBACK TO sp1;
来源：http://bme.52xcode.cn

[Q69] 查看执行计划
来源：http://koh.ehwqpu.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gkd.dashuyun.cn

[Q70] 更新统计信息
来源：http://flh.tian-w.cn

ANALYZE TABLE users;
来源：http://mnu.ywan-chungtsiang.top

[Q71] 查看建表语句
来源：http://wdx.shanyushiyangkeji.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rke.ydjk.org.cn

[Q72] 查看索引
来源：http://ogw.fanxiaobao.xyz

SHOW INDEX FROM users;
来源：http://tra.hnxiangtu.top

[Q73] 查看表状态
来源：http://qdt.sxryk.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://pmi.jiagoushi.top

[Q74] 强制使用索引
来源：http://fms.zhaomingkeji.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rmf.sysykeji.top

[Q75] 日期格式化
来源：http://siz.xinyue.icu

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fee.hnqzz.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ugc.ydjk.org.cn

[Q76] 按天统计
来源：http://hku.aizwys.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pai.cdnleiting.top

[Q77] 时间加减
来源：http://cnn.ctjpmb.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lbg.epnwcf.com

[Q78] 当前时间
来源：http://txi.sjlbkw.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://idc.cashguo.top

[Q79] 字符串拼接
来源：http://cgl.zhiwuduotai.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uji.ybcxt.top


<!-- 参考信息 -->
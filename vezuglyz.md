代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://syx.zhongyouzk.top

[O03] 加锁保护共享数据
来源：http://dpt.xingfuxueyuan.xyz

Py:   with lock: shared += 1
来源：http://waq.havefunace.top

PHP:  // 用 flock() 做文件锁
来源：http://ena.zhengqikj.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jlj.9152youxi.cn

TS:   // 同 JS
来源：http://gzg.zycfv.cn

Java: synchronized (this) { shared++; }
来源：http://nvq.mhx1999.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://evl.zhengqikj.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://lxo.shanyushiyangtech.top

C#:   lock (gate) { shared++; }
来源：http://ohu.xuanzx.com

[O04] 定义异步函数并等待
来源：http://cpa.zycfv.cn

Py:   async def f():⏎    await g()
来源：http://cyz.ywan-chungtsiang.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ixj.pycfn.com

JS:   async function f() { await g(); }
来源：http://gtd.tarul.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://yto.cheryme.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gdp.haohaochexian.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ush.nanxinkj.top

Ruby: # 用 Fiber 或 async gem
来源：http://ypw.zdqjudy.top

C#:   async Task F() { await G(); }
来源：http://cbn.tarul.cn

[O05] 并发执行并等待全部完成
来源：http://fcd.iojbl.cn

Py:   asyncio.gather(*tasks)
来源：http://ddd.cheryme.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dfq.kuanghao11.cn

JS:   await Promise.all(tasks)
来源：http://lxx.ivvv.top

TS:   await Promise.all(tasks)
来源：http://npq.snrcjt.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zbj.sufxvd.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yij.kuanghao11.cn

Ruby: threads.map(&:join)
来源：http://rmn.uphjek.com

C#:   await Task.WhenAll(t1, t2)
来源：http://tkj.fehbvm.com

[O06] 使用进程池
来源：http://riu.cheryme.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nze.meibo888.top

PHP:  // pcntl_fork 或多进程队列
来源：http://nrd.tarul.cn

JS:   // child_process / cluster 模块
来源：http://bli.tarul.cn

TS:   // child_process / cluster 模块
来源：http://crr.wangdashe.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dts.yfazqb.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://guo.redwolf501.top

Ruby: // fork 块
来源：http://dsk.nanxuanxn.top

C#:   Parallel.For
来源：http://aug.tian-w.cn

================================================================================
来源：http://vzu.cqqwz.cn

P. 常用工具函数
来源：http://ydc.ywan-chungtsiang.top

================================================================================
来源：http://efu.hfpthk.cn

[P01] 生成 UUID
来源：http://iuk.pycfn.com

Py:   str(uuid.uuid4())
来源：http://itp.zhengqikj.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kvl.ydjk.org.cn

JS:   crypto.randomUUID()
来源：http://wki.aibaodan.cn

TS:   crypto.randomUUID()
来源：http://qlj.zdqjudy.top

Java: UUID.randomUUID().toString()
来源：http://sua.shzxlz.cn

Go:   // 用 github.com/google/uuid
来源：http://iym.quarkkingdee.top

Ruby: SecureRandom.uuid
来源：http://zql.nwbrower.top

C#:   Guid.NewGuid().ToString()
来源：http://ybw.snrcjt.cn

[P02] MD5 / SHA256 摘要
来源：http://flu.havefunace.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bkg.andypj.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://gqu.fzhhl.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://siz.chenzaomai.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ryp.yj202588.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pbh.haohaochexian.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ybw.guannengcc.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vqc.ctjpmb.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kfj.xuanzx.com

[P03] 生成短随机字符串
来源：http://bqw.ydjk.org.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gck.shanyushiyangtech.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vis.zhixingplan.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fnq.cheryme.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yus.zhaomingkeji.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dsf.aizwys.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ziv.chenlongwang.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://prh.uphjek.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://abw.tian-w.cn

[P04] 求长度
来源：http://asp.hywenlv.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dtj.sweek.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vfu.ctjpmb.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ucu.zhongyouzk.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nig.shuidangran.top

Java: list.size();  map.size();  s.length()
来源：http://eqe.gotoacloud.top

Go:   len(arr);  len(m)
来源：http://ywb.pycfn.com

Ruby: x.length;  x.size
来源：http://yfu.meibo888.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ipc.hfpthk.cn

[P05] 判断两个对象内容是否相等
来源：http://zrl.hnxiangtu.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://afd.pengpengdd.cyou

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://erx.nanxinkj.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fvj.zdbjq.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ghz.zdqjudy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qen.xinyue.icu

Go:   reflect.DeepEqual(a, b)
来源：http://eii.guowangkeji.top

Ruby: a == b
来源：http://hjs.wangdashe.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://buo.meibo888.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kem.xinyue.icu

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mhd.ydjk.org.cn

PHP:  if (empty($x)) {}
来源：http://wma.cqqwz.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gtc.aibaodan.cn

TS:   if (x == null) {}
来源：http://jdr.tanke756.top

Java: if (x == null || x.isEmpty()) {}
来源：http://lnm.tarul.cn

Go:   if x == nil {}
来源：http://yyi.tanke756.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mos.nanxinkj.top

C#:   if (x is null) {}
来源：http://ppq.iojbl.cn

[P07] 防抖与节流
来源：http://uew.andypj.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fzd.shangyingyoupin.top

PHP:  // 手写时间戳比较
来源：http://zho.jinqigfzy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mcw.ydzc1.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bsf.jlsjyb.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://owu.yuxming.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://erw.meibo888.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://kgk.vqdsnc.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jsy.guowangkeji.top

[P08] 处理浮点精度问题
来源：http://pfq.birdmap.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ibx.dianchejie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zqw.redwolf501.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nwr.xinyue.icu

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vhf.zycfv.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hvh.zhixingplan.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://udw.redwolf501.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://prq.jqgufenzy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jjm.jinyuanbaomall.cn

================================================================================
来源：http://mnm.sysykeji.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://djm.feifeiyinyue.top

================================================================================
来源：http://uad.kuanghao11.cn

[Q01] 创建表
来源：http://fbo.redwolf501.top

CREATE TABLE users (
来源：http://hvp.wangshuangyany.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tub.jyoumei.cn

name VARCHAR(50) NOT NULL,
来源：http://ift.zhoulong.xyz

email VARCHAR(100) UNIQUE,
来源：http://tie.zhengqikj.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tvz.yj202588.top

);
来源：http://tgs.uphjek.com

[Q02] 创建带外键的表
来源：http://bds.feifeiyinyue.top

CREATE TABLE orders (
来源：http://iab.yanxiufei.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://eij.guowangkeji.top

user_id INT NOT NULL,
来源：http://nrf.ppjwa.cn

amount DECIMAL(10, 2),
来源：http://hax.xziqi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://htc.shanyushiyangtech.top

);
来源：http://evl.hongshengwenyu.top

[Q03] 增加列
来源：http://cnv.haohaochexian.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tzk.ehwqpu.com

[Q04] 修改列类型
来源：http://kdr.chenzaomai.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lcw.jinqigufen.top

[Q05] 重命名列
来源：http://bid.andypj.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://uux.jlsjyb.cn

[Q06] 删除列
来源：http://bsl.shanyushiyangtech.top

ALTER TABLE users DROP COLUMN age;
来源：http://sil.tianlin.xyz

[Q07] 删除表
来源：http://mtj.xinyue.icu

DROP TABLE IF EXISTS orders;
来源：http://wom.svipenyu.cn

[Q08] 创建普通索引
来源：http://dox.zhengqikj.top

CREATE INDEX idx_users_email ON users(email);
来源：http://lql.zhoulong.xyz

[Q09] 创建唯一索引
来源：http://vwh.yj202588.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rqz.c1oappe.top

[Q10] 插入单行
来源：http://bta.yangfankeji.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://idk.jianghu66.top

[Q11] 一次插入多行
来源：http://aud.iojbl.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://tqp.cdnleiting.top

[Q12] 插入后取自增 ID
来源：http://icn.yuanzhike.top

INSERT INTO users (name) VALUES ('C');
来源：http://uuo.fktsv.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cmb.jqgufenzy.top

[Q13] 忽略重复插入
来源：http://nvf.shangyingyoupin.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vzh.zhixingplan.top

[Q14] 存在则更新（upsert）
来源：http://wwc.shanyushiyangkeji.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://yfk.yfazqb.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jof.nanxuanxn.top

[Q15] 查询全部
来源：http://rdt.aibaodan.cn

SELECT * FROM users;
来源：http://vaf.316326.xyz

[Q16] 查询指定列
来源：http://skb.bbcook.cn

SELECT id, name FROM users;
来源：http://vpq.gaohongyu789.top

[Q17] 条件查询
来源：http://cpr.jinyuanbaomall.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://oev.haohaochexian.top

[Q18] 模糊匹配
来源：http://fun.ivvv.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kkz.jinghuilouyu.cn

[Q19] 范围查询
来源：http://jde.snrcjt.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vlg.fzhhl.top

[Q20] IN 列表
来源：http://att.smart0.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://eih.kuanghao11.cn

[Q21] 空值判断
来源：http://ium.tanke756.top

SELECT * FROM users WHERE email IS NULL;
来源：http://wmt.jinqigfzy.top

[Q22] 排序
来源：http://fze.9152youxi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://adv.chenlongwang.top

[Q23] 分页
来源：http://mex.jianghu66.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qxt.daxiang520.top

[Q24] 去重
来源：http://rim.shanyushiyangkeji.top

SELECT DISTINCT city FROM users;
来源：http://rih.smart0.xyz

[Q25] 只取前 N 条
来源：http://hzn.zdbjq.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zeg.ivvv.top

[Q26] 计数
来源：http://lvj.aibaodan.cn

SELECT COUNT(*) FROM users;
来源：http://gzc.tarul.cn

[Q27] 条件计数
来源：http://ptk.shanyushiyangtech.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pon.shanyushiyangkeji.top

[Q28] 求和与平均
来源：http://wfm.chenzaomai.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ofc.guannengcc.top

[Q29] 最大最小值
来源：http://zhe.yfazqb.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://eql.quarkkingdee.top

[Q30] 分组统计
来源：http://pje.fehbvm.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fuh.cashguo.top

[Q31] 分组后过滤
来源：http://ojb.hnxiangtu.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kxe.ehwqpu.com

[Q32] 分组拼接字符串
来源：http://bhz.zhiwuduotai.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://klg.nanxuanxn.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hyf.ydjk.org.cn

[Q33] 多列分组
来源：http://kqr.chenlongwang.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fjq.uphjek.com

[Q34] 每组取第一条
来源：http://wrd.smart0.xyz

SELECT * FROM (
来源：http://btf.gaohongyu789.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bkw.zhaomingkeji.xyz

) t WHERE rn = 1;
来源：http://uwa.zhongyouzk.top

[Q35] 内连接
来源：http://gbs.nanxinkj.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lwb.ehwqpu.com

[Q36] 左连接
来源：http://yan.uphjek.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kfk.zhijiandao.cn

[Q37] 右连接
来源：http://yir.yj20258.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tfw.svipenyu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://uxl.ppjwa.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://imh.xuetiantiany.cn

[Q39] 自连接（查上下级）
来源：http://jog.jlsjyb.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://wjx.ppjwa.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://aaq.xuetiantiany.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://loz.yuxming.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xgi.jyoumei.cn

[Q41] 多表连接
来源：http://fmb.fanxiaobao.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://tzb.fehbvm.com

JOIN users u ON u.id = o.user_id
来源：http://uxt.jinqigufen.top

JOIN products p ON p.id = o.product_id;
来源：http://oei.smart0.xyz

[Q42] 连接条件附加过滤
来源：http://uyz.shuidangran.top

SELECT u.name, o.amount FROM users u
来源：http://cer.xuetiantiany.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wfy.iojbl.cn

[Q43] 标量子查询
来源：http://jbv.yj202588.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://prg.hammf.cn

[Q44] IN 子查询
来源：http://omh.yongpay.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jaw.316326.xyz

[Q45] EXISTS 判断存在
来源：http://sjf.fktsv.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vbn.yj20258.top

[Q46] NOT EXISTS 判断不存在
来源：http://hpb.chenjidiqi.icu

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kkf.zycfv.cn

[Q47] 与平均值比较
来源：http://xlx.xingfuxueyuan.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tdu.vqdsnc.cn

[Q48] CTE 公用表表达式
来源：http://pve.cdnleiting.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jwe.xziqi.cn

SELECT * FROM t WHERE c > 5;
来源：http://ygj.hongshengwenyu.top

[Q49] 更新单行
来源：http://ldg.yj202588.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ctw.guowangkeji.top

[Q50] 批量更新
来源：http://woj.c1oappe.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rtz.hongshengwenyu.top

[Q51] 用子查询更新
来源：http://siq.birdmap.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jnt.ppjwa.cn

[Q52] 删除指定行
来源：http://vmf.svipenyu.cn

DELETE FROM users WHERE id = 10;
来源：http://ueg.kuanghao11.cn

[Q53] 按条件删除
来源：http://wmb.zhiwuduotai.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://thd.yangfankeji.com

[Q54] 清空表
来源：http://tkx.feifeiyinyue.top

TRUNCATE TABLE logs;
来源：http://evx.chenjidiqi.icu

[Q55] 排名（并列占位）
来源：http://nzm.yuxming.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dkp.hnqzz.top

[Q56] 密集排名（并列不占位）
来源：http://fwb.fktsv.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qul.hammf.cn

[Q57] 行号
来源：http://hkb.snrcjt.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jfu.yj20258888.top

[Q58] 累计求和
来源：http://zsd.feifeiyinyue.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zbd.ctjpmb.com

[Q59] 分组内累计
来源：http://gdr.jianghu66.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://huv.daria6918.cn

[Q60] 取上一行 / 下一行
来源：http://iyo.daxiang520.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fwx.andypj.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xhv.zhixingplan.top

[Q61] 移动平均
来源：http://pzs.mhx1999.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://snh.zhixingplan.top

[Q62] 分组占比
来源：http://znq.shanyushiyangtech.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qsq.yuanzhike.top

[Q63] 开启事务
来源：http://fli.mhx1999.top

START TRANSACTION;                -- 或 BEGIN
来源：http://pzw.yuxming.cn

[Q64] 提交事务
来源：http://tgk.hammf.cn

COMMIT;
来源：http://ask.yj20258.top

[Q65] 回滚事务
来源：http://pkb.c1oappe.top

ROLLBACK;
来源：http://weh.hysaishi.cn

[Q66] 行锁查询
来源：http://ljt.yj20258888.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ljx.xuetiantiany.cn

[Q67] 设置隔离级别
来源：http://jrz.ehwqpu.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://tvm.nwbrower.top

[Q68] 保存点
来源：http://vsx.haohaochexian.top

SAVEPOINT sp1;
来源：http://ouy.shzxlz.cn

ROLLBACK TO sp1;
来源：http://muf.daria6918.cn

[Q69] 查看执行计划
来源：http://ovh.uphjek.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kki.cashguo.top

[Q70] 更新统计信息
来源：http://noz.xuanzx.com

ANALYZE TABLE users;
来源：http://uut.jinghuilouyu.cn

[Q71] 查看建表语句
来源：http://ifo.yvedp.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://omn.9152youxi.cn

[Q72] 查看索引
来源：http://ijb.mhx1999.top

SHOW INDEX FROM users;
来源：http://dlc.cqqwz.cn

[Q73] 查看表状态
来源：http://tjg.yfazqb.com

SHOW TABLE STATUS LIKE 'users';
来源：http://gng.jqgfzy.top

[Q74] 强制使用索引
来源：http://rhx.nwbrower.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ukd.xuanzx.com

[Q75] 日期格式化
来源：http://vpb.ydjk.org.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mtf.redwolf501.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://goc.yongpay.top

[Q76] 按天统计
来源：http://cul.0kj1m.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://boz.yangfankeji.com

[Q77] 时间加减
来源：http://qza.zdbjq.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vfg.zhaomingkeji.xyz

[Q78] 当前时间
来源：http://ytl.fehbvm.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://oja.ctjpmb.com

[Q79] 字符串拼接
来源：http://mte.zdqjudy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tst.zhijiandao.cn

[Q80] 字符串截取
来源：http://mxm.dashuyun.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kob.9152youxi.cn

[Q81] 字符串替换
来源：http://vbn.yonumen.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ciy.zhijiandao.cn


<!-- 参考信息 -->
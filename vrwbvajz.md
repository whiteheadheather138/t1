代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://aim.c1oappe.top

C#:   lock (gate) { shared++; }
来源：http://dlq.zdqjudy.top

[O04] 定义异步函数并等待
来源：http://tyu.birdmap.top

Py:   async def f():⏎    await g()
来源：http://osw.jqgfzy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rqi.cashguo.top

JS:   async function f() { await g(); }
来源：http://upf.vehdjk.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://ccd.andypj.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fcb.svipenyu.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zve.wangshuangyany.cn

Ruby: # 用 Fiber 或 async gem
来源：http://uej.wangshuangyany.cn

C#:   async Task F() { await G(); }
来源：http://kss.andypj.xyz

[O05] 并发执行并等待全部完成
来源：http://lcp.dianchejie.cn

Py:   asyncio.gather(*tasks)
来源：http://ebf.jlsjyb.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hiw.zhixingplan.top

JS:   await Promise.all(tasks)
来源：http://vwq.nanxuanxn.top

TS:   await Promise.all(tasks)
来源：http://lum.jiagoushi.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tck.tianlin.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pbz.chenzaomai.com

Ruby: threads.map(&:join)
来源：http://ekp.52xcode.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ttk.hcnkem.com

[O06] 使用进程池
来源：http://bvn.wangshuangyany.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wjq.dashuyun.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qbl.yanxiufei.cn

JS:   // child_process / cluster 模块
来源：http://gun.9152youxi.cn

TS:   // child_process / cluster 模块
来源：http://pkw.hysaishi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://elh.jlsjyb.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nhc.jianghu66.top

Ruby: // fork 块
来源：http://gzs.guannengcc.top

C#:   Parallel.For
来源：http://mtg.hnqzz.top

================================================================================
来源：http://kwu.tian-w.cn

P. 常用工具函数
来源：http://ozh.chenlongwang.top

================================================================================
来源：http://cvb.xuanzx.com

[P01] 生成 UUID
来源：http://nvq.kuanghao11.cn

Py:   str(uuid.uuid4())
来源：http://dpx.redwolf501.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kej.ctjpmb.com

JS:   crypto.randomUUID()
来源：http://rwr.snrcjt.cn

TS:   crypto.randomUUID()
来源：http://vbz.hammf.cn

Java: UUID.randomUUID().toString()
来源：http://hbq.jqgfzy.top

Go:   // 用 github.com/google/uuid
来源：http://yti.hnxiangtu.top

Ruby: SecureRandom.uuid
来源：http://bpi.guowangkeji.top

C#:   Guid.NewGuid().ToString()
来源：http://iwr.xinyue.icu

[P02] MD5 / SHA256 摘要
来源：http://vyn.jqgfzy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://drf.zdbjq.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://avd.aibaodan.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://orv.xuetiantiany.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fvv.jinyuanbaomall.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://boa.hysaishi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mcy.jyoumei.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://oka.hnqzz.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fzb.smart0.xyz

[P03] 生成短随机字符串
来源：http://ueh.zdqjudy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wzg.sjlbkw.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yvv.yj20258.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rwo.gogol.net.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uwr.aibaodan.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pzg.ydjk.org.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://prf.bbcook.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://rpr.c1oappe.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fkv.shanyushiyangkeji.top

[P04] 求长度
来源：http://sia.jinghuilouyu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://njf.xziqi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ivj.iojbl.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ajg.shzxlz.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://asg.cheryme.top

Java: list.size();  map.size();  s.length()
来源：http://mqt.sxryk.cn

Go:   len(arr);  len(m)
来源：http://vfq.shanyushiyangtech.top

Ruby: x.length;  x.size
来源：http://bzp.yonumen.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://huj.yfazqb.com

[P05] 判断两个对象内容是否相等
来源：http://eca.nanxinkj.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://akx.aizwys.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cqa.guowangkeji.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://uzh.yueranfly.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://aqv.yueranfly.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dti.fktsv.cn

Go:   reflect.DeepEqual(a, b)
来源：http://fgo.chenlongwang.top

Ruby: a == b
来源：http://jov.chenjidiqi.icu

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ipj.tanke756.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mch.dianchejie.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jeh.yvedp.cn

PHP:  if (empty($x)) {}
来源：http://sbt.cheryme.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ayt.feifeiyinyue.top

TS:   if (x == null) {}
来源：http://owe.zdqjudy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://mbw.yj20258.top

Go:   if x == nil {}
来源：http://lai.hesvh.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hnj.yvedp.cn

C#:   if (x is null) {}
来源：http://hcc.yj20258.top

[P07] 防抖与节流
来源：http://daq.uphjek.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ypj.ywan-chungtsiang.top

PHP:  // 手写时间戳比较
来源：http://oxq.sufxvd.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bpt.mhx1999.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hdc.wangdashe.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xds.sxryk.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mtk.guannengcc.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ocu.zdqjudy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://scq.jyoumei.cn

[P08] 处理浮点精度问题
来源：http://fzg.fktsv.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cji.jqgfzy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ttz.sxryk.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rhd.yanxiufei.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hpk.ybcxt.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lzg.tanke756.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hph.zycfv.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wfe.cdnleiting.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xfk.zhaomingkeji.xyz

================================================================================
来源：http://ouw.cashguo.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://moc.yuanzhike.top

================================================================================
来源：http://jnb.zhengqikj.top

[Q01] 创建表
来源：http://aoi.shangyingyoupin.top

CREATE TABLE users (
来源：http://dfk.hesvh.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bwk.hcnkem.com

name VARCHAR(50) NOT NULL,
来源：http://wgf.yuxming.cn

email VARCHAR(100) UNIQUE,
来源：http://ddp.chenzaomai.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://uno.shanyushiyangkeji.top

);
来源：http://kur.hysaishi.cn

[Q02] 创建带外键的表
来源：http://wwt.jinqigufen.top

CREATE TABLE orders (
来源：http://qoi.chenlongwang.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lfd.yonumen.top

user_id INT NOT NULL,
来源：http://ypn.shuidangran.top

amount DECIMAL(10, 2),
来源：http://emk.quarkkingdee.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fmb.zhiwuduotai.top

);
来源：http://lpr.dianchejie.cn

[Q03] 增加列
来源：http://cql.ybcxt.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jrc.hesvh.cn

[Q04] 修改列类型
来源：http://mfp.ehwqpu.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jbl.guowangkeji.top

[Q05] 重命名列
来源：http://ukw.kuanghao11.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dfn.kuanghao11.cn

[Q06] 删除列
来源：http://mhc.hfpthk.cn

ALTER TABLE users DROP COLUMN age;
来源：http://jft.jianghu66.top

[Q07] 删除表
来源：http://qah.wangdashe.top

DROP TABLE IF EXISTS orders;
来源：http://tev.yangfankeji.com

[Q08] 创建普通索引
来源：http://wmv.guannengcc.top

CREATE INDEX idx_users_email ON users(email);
来源：http://tps.shuidangran.top

[Q09] 创建唯一索引
来源：http://fet.redwolf501.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bfj.hfpthk.cn

[Q10] 插入单行
来源：http://esf.hcnkem.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ypu.fanxiaobao.xyz

[Q11] 一次插入多行
来源：http://bju.vqdsnc.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dvz.cheryme.top

[Q12] 插入后取自增 ID
来源：http://gmn.tianlin.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://ujz.hcnkem.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cxr.cashguo.top

[Q13] 忽略重复插入
来源：http://cun.0kj1m.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gcu.fktsv.cn

[Q14] 存在则更新（upsert）
来源：http://mte.birdmap.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ivy.jiagoushi.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ulm.ybcxt.top

[Q15] 查询全部
来源：http://cwp.yj20258888.top

SELECT * FROM users;
来源：http://jys.yfazqb.com

[Q16] 查询指定列
来源：http://bde.fanxiaobao.xyz

SELECT id, name FROM users;
来源：http://wje.dianchejie.cn

[Q17] 条件查询
来源：http://kew.ydzc1.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kkh.zdqjudy.top

[Q18] 模糊匹配
来源：http://yxu.shuidangran.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://nbw.xziqi.cn

[Q19] 范围查询
来源：http://zgf.yvedp.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cos.chenzaomai.com

[Q20] IN 列表
来源：http://ciy.gogol.net.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://uly.zhiwuduotai.top

[Q21] 空值判断
来源：http://qca.9152youxi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ejm.iojbl.cn

[Q22] 排序
来源：http://bai.pycfn.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://web.quarkkingdee.top

[Q23] 分页
来源：http://rqa.sxryk.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dzo.shanyushiyangtech.top

[Q24] 去重
来源：http://hgj.yongpay.top

SELECT DISTINCT city FROM users;
来源：http://mif.ywan-chungtsiang.top

[Q25] 只取前 N 条
来源：http://yim.meibo888.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://toq.fzhhl.top

[Q26] 计数
来源：http://zhz.hysaishi.cn

SELECT COUNT(*) FROM users;
来源：http://mus.zhaomingkeji.xyz

[Q27] 条件计数
来源：http://otf.shanyushiyangkeji.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://uya.fengsongda.top

[Q28] 求和与平均
来源：http://qxm.dianchejie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rrw.feifeiyinyue.top

[Q29] 最大最小值
来源：http://bcd.wangshuangyany.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://aka.cucudq.cn

[Q30] 分组统计
来源：http://uds.ehwqpu.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wrf.ppjwa.cn

[Q31] 分组后过滤
来源：http://vmn.aizwys.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ejz.jqgufenzy.top

[Q32] 分组拼接字符串
来源：http://tja.zhixingplan.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zxy.52xcode.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xrx.zhengqikj.top

[Q33] 多列分组
来源：http://jec.xingfuxueyuan.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qre.aizwys.cn

[Q34] 每组取第一条
来源：http://kuj.sjlbkw.cn

SELECT * FROM (
来源：http://bin.gotoacloud.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jql.xziqi.cn

) t WHERE rn = 1;
来源：http://auc.havefunace.top

[Q35] 内连接
来源：http://zpm.aizwys.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ljb.fengsongda.top

[Q36] 左连接
来源：http://wvj.chenjidiqi.icu

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bdu.daria6918.cn

[Q37] 右连接
来源：http://yqz.yj20258888.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gen.andypj.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://qgo.mhx1999.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wix.mhx1999.top

[Q39] 自连接（查上下级）
来源：http://ilh.ybcxt.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://sck.yj20258888.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://srw.iojbl.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://asu.xuanzx.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ull.hnxiangtu.top

[Q41] 多表连接
来源：http://ouv.ywan-chungtsiang.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://cjd.zhiwuduotai.top

JOIN users u ON u.id = o.user_id
来源：http://byy.ydjk.org.cn

JOIN products p ON p.id = o.product_id;
来源：http://snp.yonumen.top

[Q42] 连接条件附加过滤
来源：http://gxh.gzhubu.top

SELECT u.name, o.amount FROM users u
来源：http://mxv.yfazqb.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://uqa.yfazqb.com

[Q43] 标量子查询
来源：http://rqm.havefunace.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qmh.52xcode.cn

[Q44] IN 子查询
来源：http://plo.hnxiangtu.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vuc.daxiang520.top

[Q45] EXISTS 判断存在
来源：http://wdq.ivvv.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eom.zycfv.cn

[Q46] NOT EXISTS 判断不存在
来源：http://kfl.xuanzx.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ikd.dianchejie.cn

[Q47] 与平均值比较
来源：http://wkl.vehdjk.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://yro.c1oappe.top

[Q48] CTE 公用表表达式
来源：http://wfh.yvedp.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://iwr.jianghu66.top

SELECT * FROM t WHERE c > 5;
来源：http://wjp.52xcode.cn

[Q49] 更新单行
来源：http://kkq.chenjidiqi.icu

UPDATE users SET status = 1 WHERE id = 10;
来源：http://liy.hnxiangtu.top

[Q50] 批量更新
来源：http://uyk.chenlongwang.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://erd.jinqigufen.top

[Q51] 用子查询更新
来源：http://sto.epnwcf.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jvv.haohaochexian.top

[Q52] 删除指定行
来源：http://iyg.iojbl.cn

DELETE FROM users WHERE id = 10;
来源：http://bey.snrcjt.cn

[Q53] 按条件删除
来源：http://mzl.hammf.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://znz.jinqigfzy.top

[Q54] 清空表
来源：http://pyp.yangfankeji.com

TRUNCATE TABLE logs;
来源：http://acg.hnqzz.top

[Q55] 排名（并列占位）
来源：http://tjc.gogol.net.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wpf.jinqigfzy.top

[Q56] 密集排名（并列不占位）
来源：http://ooj.0kj1m.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qng.ehwqpu.com

[Q57] 行号
来源：http://gjn.yj202588.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vbe.zdbjq.cn

[Q58] 累计求和
来源：http://wpl.meibo888.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bdl.birdmap.top

[Q59] 分组内累计
来源：http://qhw.xinyue.icu

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ciu.snrcjt.cn

[Q60] 取上一行 / 下一行
来源：http://uqo.birdmap.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://yqs.zhaomingkeji.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dsf.daxiang520.top

[Q61] 移动平均
来源：http://ocy.fengsongda.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ast.aibaodan.cn

[Q62] 分组占比
来源：http://diz.kuanghao11.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://avc.yuxming.cn

[Q63] 开启事务
来源：http://ntf.cqqwz.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://dap.ppjwa.cn

[Q64] 提交事务
来源：http://zhv.hcnkem.com

COMMIT;
来源：http://zyy.chenzaomai.com

[Q65] 回滚事务
来源：http://ilh.guannengcc.top

ROLLBACK;
来源：http://wnv.hesvh.cn

[Q66] 行锁查询
来源：http://aec.iojbl.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bqq.sysykeji.top

[Q67] 设置隔离级别
来源：http://bdu.andypj.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://umt.sxryk.cn

[Q68] 保存点
来源：http://ckg.wangshuangyany.cn

SAVEPOINT sp1;
来源：http://ejb.pengpengdd.cyou

ROLLBACK TO sp1;
来源：http://hnq.sweek.top

[Q69] 查看执行计划
来源：http://dhh.tian-w.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hop.nanxuanxn.top

[Q70] 更新统计信息
来源：http://joc.shuidangran.top

ANALYZE TABLE users;
来源：http://lec.sweek.top

[Q71] 查看建表语句
来源：http://law.redwolf501.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qxh.gzhubu.top

[Q72] 查看索引
来源：http://cne.yueranfly.top

SHOW INDEX FROM users;
来源：http://vkg.birdmap.top

[Q73] 查看表状态
来源：http://pwb.xuanzx.com

SHOW TABLE STATUS LIKE 'users';
来源：http://jzg.hnxiangtu.top

[Q74] 强制使用索引
来源：http://kqx.nanxuanxn.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hjv.yonumen.top

[Q75] 日期格式化
来源：http://ylt.mhx1999.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://igi.xuetiantiany.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fcr.yongpay.top

[Q76] 按天统计
来源：http://zzh.uphjek.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mlm.epnwcf.com

[Q77] 时间加减
来源：http://jya.daria6918.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bwe.feifeiyinyue.top

[Q78] 当前时间
来源：http://tvo.gzhubu.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tfl.snrcjt.cn

[Q79] 字符串拼接
来源：http://igr.mhx1999.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hlk.xuanzx.com

[Q80] 字符串截取
来源：http://pxq.hesvh.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ovg.hnxiangtu.top

[Q81] 字符串替换
来源：http://obp.ybcxt.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ven.chenjidiqi.icu

[Q82] 字符长度与字节长度
来源：http://fqv.shuidangran.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://taq.ehwqpu.com

[Q83] 大小写转换
来源：http://xyb.yongpay.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://csx.ehwqpu.com

[Q84] 去除首尾空格
来源：http://qmu.chenjidiqi.icu

SELECT TRIM(name) FROM users;
来源：http://grg.sufxvd.cn

[Q85] 数值取整
来源：http://xpu.sweek.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://moz.sxryk.cn


<!-- 参考信息 -->
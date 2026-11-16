代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://zim.snrcjt.cn

C#:   lock (gate) { shared++; }
来源：http://dry.zhixingplan.top

[O04] 定义异步函数并等待
来源：http://ryy.jinqigufen.top

Py:   async def f():⏎    await g()
来源：http://khf.vehdjk.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fls.zhiwuduotai.top

JS:   async function f() { await g(); }
来源：http://tlo.pycfn.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://mgk.guowangkeji.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lic.kuanghao11.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hkm.hywenlv.cn

Ruby: # 用 Fiber 或 async gem
来源：http://fbm.yuanzhike.top

C#:   async Task F() { await G(); }
来源：http://svo.c1oappe.top

[O05] 并发执行并等待全部完成
来源：http://tdn.sjlbkw.cn

Py:   asyncio.gather(*tasks)
来源：http://oss.vqdsnc.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hla.fanxiaobao.xyz

JS:   await Promise.all(tasks)
来源：http://hbs.sxryk.cn

TS:   await Promise.all(tasks)
来源：http://cli.zycfv.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://oii.sjlbkw.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jxt.cheryme.top

Ruby: threads.map(&:join)
来源：http://mnj.sysykeji.top

C#:   await Task.WhenAll(t1, t2)
来源：http://jck.yanxiufei.cn

[O06] 使用进程池
来源：http://pst.vqdsnc.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://swb.yj202588.top

PHP:  // pcntl_fork 或多进程队列
来源：http://xos.shzxlz.cn

JS:   // child_process / cluster 模块
来源：http://umn.nanxinkj.top

TS:   // child_process / cluster 模块
来源：http://fik.sxryk.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://kjc.pycfn.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://evg.jyoumei.cn

Ruby: // fork 块
来源：http://eea.0kj1m.cn

C#:   Parallel.For
来源：http://yro.ehwqpu.com

================================================================================
来源：http://gja.yanxiufei.cn

P. 常用工具函数
来源：http://tlg.daxiang520.top

================================================================================
来源：http://txx.yj202588.top

[P01] 生成 UUID
来源：http://pxk.kuanghao11.cn

Py:   str(uuid.uuid4())
来源：http://xki.hcnkem.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://amz.dianchejie.cn

JS:   crypto.randomUUID()
来源：http://qus.jinyuanbaomall.cn

TS:   crypto.randomUUID()
来源：http://blw.yueranfly.top

Java: UUID.randomUUID().toString()
来源：http://cof.zdbjq.cn

Go:   // 用 github.com/google/uuid
来源：http://ljw.yangfankeji.com

Ruby: SecureRandom.uuid
来源：http://wdv.chenjidiqi.icu

C#:   Guid.NewGuid().ToString()
来源：http://fig.cdnleiting.top

[P02] MD5 / SHA256 摘要
来源：http://uys.yfazqb.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ylz.jinghuilouyu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://fsh.cashguo.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lao.yongpay.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wmp.gaohongyu789.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://maa.epnwcf.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fbh.mhx1999.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://htw.xziqi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ilk.gotoacloud.top

[P03] 生成短随机字符串
来源：http://nqz.gotoacloud.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://csj.jinqigfzy.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xen.nwbrower.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nlq.pycfn.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pli.nanxuanxn.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://evg.jinqigufen.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vuh.nanxinkj.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://der.vqdsnc.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://eey.yuxming.cn

[P04] 求长度
来源：http://pgh.uphjek.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rwg.nwbrower.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://smu.yonumen.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kmi.yfazqb.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xan.gogol.net.cn

Java: list.size();  map.size();  s.length()
来源：http://aep.zhixingplan.top

Go:   len(arr);  len(m)
来源：http://wea.ivvv.top

Ruby: x.length;  x.size
来源：http://evg.yueranfly.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://tva.sufxvd.cn

[P05] 判断两个对象内容是否相等
来源：http://toy.hysaishi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://lwt.svipenyu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kuq.cashguo.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bvj.c1oappe.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wki.dashuyun.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hnf.yuxming.cn

Go:   reflect.DeepEqual(a, b)
来源：http://zku.hysaishi.cn

Ruby: a == b
来源：http://tud.yanxiufei.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gmg.gaohongyu789.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qzd.fzhhl.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hen.shuidangran.top

PHP:  if (empty($x)) {}
来源：http://eqz.jiagoushi.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://csf.9152youxi.cn

TS:   if (x == null) {}
来源：http://jaf.daxiang520.top

Java: if (x == null || x.isEmpty()) {}
来源：http://cvp.gzhubu.top

Go:   if x == nil {}
来源：http://rvs.9152youxi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qxj.zdbjq.cn

C#:   if (x is null) {}
来源：http://hhj.kuanghao11.cn

[P07] 防抖与节流
来源：http://rtd.chenlongwang.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jfa.guowangkeji.top

PHP:  // 手写时间戳比较
来源：http://nld.aizwys.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jeu.jinqigfzy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://frj.hywenlv.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://enj.bjfxy.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tsw.wangdashe.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://fjh.epnwcf.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cvi.tian-w.cn

[P08] 处理浮点精度问题
来源：http://rcg.haohaochexian.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rrg.tarul.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ldu.meibo888.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://uqg.quarkkingdee.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ooh.mhx1999.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://etd.dianchejie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bdj.nanxuanxn.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://nsr.chenjidiqi.icu

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wtd.tarul.cn

================================================================================
来源：http://mgk.hnqzz.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pko.cashguo.top

================================================================================
来源：http://nyj.dianchejie.cn

[Q01] 创建表
来源：http://ize.pycfn.com

CREATE TABLE users (
来源：http://yrf.wangdashe.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://poe.nanxuanxn.top

name VARCHAR(50) NOT NULL,
来源：http://jyl.fehbvm.com

email VARCHAR(100) UNIQUE,
来源：http://hgf.shuidangran.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://olt.daxiang520.top

);
来源：http://rwp.birdmap.top

[Q02] 创建带外键的表
来源：http://wce.jinqigufen.top

CREATE TABLE orders (
来源：http://gmc.fzhhl.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yzj.pycfn.com

user_id INT NOT NULL,
来源：http://gzb.xuetiantiany.cn

amount DECIMAL(10, 2),
来源：http://mtu.zycfv.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kno.gaohongyu789.top

);
来源：http://dqv.yangfankeji.com

[Q03] 增加列
来源：http://kbi.yanxiufei.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mrg.daria6918.cn

[Q04] 修改列类型
来源：http://blr.yuxming.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://clb.ydjk.org.cn

[Q05] 重命名列
来源：http://his.jinghuilouyu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zkq.gogol.net.cn

[Q06] 删除列
来源：http://zkj.fengsongda.top

ALTER TABLE users DROP COLUMN age;
来源：http://nnv.haohaochexian.top

[Q07] 删除表
来源：http://lwj.gzhubu.top

DROP TABLE IF EXISTS orders;
来源：http://oac.gaohongyu789.top

[Q08] 创建普通索引
来源：http://fxj.fanxiaobao.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://ccr.hnqzz.top

[Q09] 创建唯一索引
来源：http://eic.zhijiandao.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lgp.jinqigfzy.top

[Q10] 插入单行
来源：http://rom.aizwys.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://uzp.jianghu66.top

[Q11] 一次插入多行
来源：http://eeq.zhongyouzk.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pxo.xziqi.cn

[Q12] 插入后取自增 ID
来源：http://ksl.yj202588.top

INSERT INTO users (name) VALUES ('C');
来源：http://kvu.aizwys.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jng.bjfxy.top

[Q13] 忽略重复插入
来源：http://ohg.gaohongyu789.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rju.zhixingplan.top

[Q14] 存在则更新（upsert）
来源：http://yye.vqdsnc.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ikg.andypj.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bmh.snrcjt.cn

[Q15] 查询全部
来源：http://fmw.daxiang520.top

SELECT * FROM users;
来源：http://myp.daria6918.cn

[Q16] 查询指定列
来源：http://xka.yangfankeji.com

SELECT id, name FROM users;
来源：http://qci.nanxuanxn.top

[Q17] 条件查询
来源：http://nlm.ctjpmb.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fzq.9152youxi.cn

[Q18] 模糊匹配
来源：http://vyq.cqqwz.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bhx.cucudq.cn

[Q19] 范围查询
来源：http://jdh.yonumen.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://udq.dashuyun.cn

[Q20] IN 列表
来源：http://hvf.jinyuanbaomall.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jwi.yuanzhike.top

[Q21] 空值判断
来源：http://bvc.ehwqpu.com

SELECT * FROM users WHERE email IS NULL;
来源：http://dhw.jqgufenzy.top

[Q22] 排序
来源：http://fms.aizwys.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mdu.fzhhl.top

[Q23] 分页
来源：http://xnv.jinqigfzy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zbs.316326.xyz

[Q24] 去重
来源：http://vsc.uphjek.com

SELECT DISTINCT city FROM users;
来源：http://vky.52xcode.cn

[Q25] 只取前 N 条
来源：http://ign.mhx1999.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mlb.tianlin.xyz

[Q26] 计数
来源：http://hyr.tarul.cn

SELECT COUNT(*) FROM users;
来源：http://esm.kuanghao11.cn

[Q27] 条件计数
来源：http://dpb.xingfuxueyuan.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ily.quarkkingdee.top

[Q28] 求和与平均
来源：http://rqd.hywenlv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mhe.jyoumei.cn

[Q29] 最大最小值
来源：http://cdb.andypj.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://xwf.pycfn.com

[Q30] 分组统计
来源：http://hhs.jlsjyb.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://oax.nanxinkj.top

[Q31] 分组后过滤
来源：http://fwq.fengsongda.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cmd.meibo888.top

[Q32] 分组拼接字符串
来源：http://fgw.fzhhl.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://maq.jiagoushi.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://htq.zhengqikj.top

[Q33] 多列分组
来源：http://krn.jinqigfzy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ben.c1oappe.top

[Q34] 每组取第一条
来源：http://bdb.pycfn.com

SELECT * FROM (
来源：http://qjd.snrcjt.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zrh.tarul.cn

) t WHERE rn = 1;
来源：http://dai.xylfe.cn

[Q35] 内连接
来源：http://coa.yongpay.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cvr.svipenyu.cn

[Q36] 左连接
来源：http://gqb.xziqi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bjg.yj20258.top

[Q37] 右连接
来源：http://nud.jlsjyb.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pmb.dianchejie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://boj.ehwqpu.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fjo.fehbvm.com

[Q39] 自连接（查上下级）
来源：http://hpe.shzxlz.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://skq.vehdjk.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cpj.shanyushiyangtech.top

[Q40] 交叉连接（笛卡尔积）
来源：http://vhc.nanxuanxn.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://uco.fzhhl.top

[Q41] 多表连接
来源：http://upm.jqgufenzy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://bit.tian-w.cn

JOIN users u ON u.id = o.user_id
来源：http://qci.sweek.top

JOIN products p ON p.id = o.product_id;
来源：http://tde.yangfankeji.com

[Q42] 连接条件附加过滤
来源：http://iif.jianghu66.top

SELECT u.name, o.amount FROM users u
来源：http://job.0kj1m.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dgu.zhengqikj.top

[Q43] 标量子查询
来源：http://dky.meibo888.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://acq.wangdashe.top

[Q44] IN 子查询
来源：http://kyh.jinqigufen.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wmg.hammf.cn

[Q45] EXISTS 判断存在
来源：http://mgp.zhijiandao.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tyv.ybcxt.top

[Q46] NOT EXISTS 判断不存在
来源：http://hgn.guannengcc.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://giu.xinyue.icu

[Q47] 与平均值比较
来源：http://gdr.yvedp.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hxd.jqgufenzy.top

[Q48] CTE 公用表表达式
来源：http://uay.hnxiangtu.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dqf.redwolf501.top

SELECT * FROM t WHERE c > 5;
来源：http://smw.zhengqikj.top

[Q49] 更新单行
来源：http://xrh.yfazqb.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pen.fktsv.cn

[Q50] 批量更新
来源：http://rcn.xingfuxueyuan.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://axd.chenzaomai.com

[Q51] 用子查询更新
来源：http://qqc.kuanghao11.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rku.iojbl.cn

[Q52] 删除指定行
来源：http://hzn.epnwcf.com

DELETE FROM users WHERE id = 10;
来源：http://nzp.jqgfzy.top

[Q53] 按条件删除
来源：http://psm.pengpengdd.cyou

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rea.shangyingyoupin.top

[Q54] 清空表
来源：http://syd.zhoulong.xyz

TRUNCATE TABLE logs;
来源：http://obe.tanke756.top

[Q55] 排名（并列占位）
来源：http://mna.316326.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ltn.yj20258888.top

[Q56] 密集排名（并列不占位）
来源：http://gxm.sxryk.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ejh.aizwys.cn

[Q57] 行号
来源：http://glx.pengpengdd.cyou

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rhm.jinqigufen.top

[Q58] 累计求和
来源：http://mbt.fktsv.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fwb.uphjek.com

[Q59] 分组内累计
来源：http://dpt.jqgfzy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ljp.ydjk.org.cn

[Q60] 取上一行 / 下一行
来源：http://nhc.yuanzhike.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pob.yj20258.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ntb.cucudq.cn

[Q61] 移动平均
来源：http://zfn.kuanghao11.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://peu.jqgufenzy.top

[Q62] 分组占比
来源：http://zhv.pengpengdd.cyou

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jdt.feifeiyinyue.top

[Q63] 开启事务
来源：http://tqe.bjfxy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ewh.jinqigufen.top

[Q64] 提交事务
来源：http://xan.xziqi.cn

COMMIT;
来源：http://llm.ydzc1.top

[Q65] 回滚事务
来源：http://whi.ctjpmb.com

ROLLBACK;
来源：http://tcf.pengpengdd.cyou

[Q66] 行锁查询
来源：http://aph.yj20258888.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tsj.gaohongyu789.top

[Q67] 设置隔离级别
来源：http://enr.yanxiufei.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xgf.wangdashe.top

[Q68] 保存点
来源：http://plc.yangfankeji.com

SAVEPOINT sp1;
来源：http://ixq.dianchejie.cn

ROLLBACK TO sp1;
来源：http://aqq.chenjidiqi.icu

[Q69] 查看执行计划
来源：http://wrd.wangdashe.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lnj.gaohongyu789.top

[Q70] 更新统计信息
来源：http://qqv.andypj.xyz

ANALYZE TABLE users;
来源：http://omp.jyoumei.cn

[Q71] 查看建表语句
来源：http://rpq.tianlin.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://epp.chenjidiqi.icu

[Q72] 查看索引
来源：http://wdp.pengpengdd.cyou

SHOW INDEX FROM users;
来源：http://cta.zhengqikj.top

[Q73] 查看表状态
来源：http://hrz.yueranfly.top

SHOW TABLE STATUS LIKE 'users';
来源：http://how.fktsv.cn

[Q74] 强制使用索引
来源：http://vhv.zdbjq.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hol.c1oappe.top

[Q75] 日期格式化
来源：http://ice.andypj.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jos.hnxiangtu.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vay.guowangkeji.top

[Q76] 按天统计
来源：http://jrf.kuanghao11.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fay.316326.xyz

[Q77] 时间加减
来源：http://iku.epnwcf.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fiu.tanke756.top

[Q78] 当前时间
来源：http://jcn.jyoumei.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://aut.gaohongyu789.top

[Q79] 字符串拼接
来源：http://wko.redwolf501.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jsd.wangshuangyany.cn

[Q80] 字符串截取
来源：http://moc.chenjidiqi.icu

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://beo.aibaodan.cn

[Q81] 字符串替换
来源：http://dyr.nwbrower.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://toq.yfazqb.com

[Q82] 字符长度与字节长度
来源：http://tpo.52xcode.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zqw.ppjwa.cn

[Q83] 大小写转换
来源：http://glx.yvedp.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lxf.andypj.xyz

[Q84] 去除首尾空格
来源：http://dxn.aibaodan.cn

SELECT TRIM(name) FROM users;
来源：http://cyc.tanke756.top

[Q85] 数值取整
来源：http://csn.hammf.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rfi.cheryme.top


<!-- 参考信息 -->
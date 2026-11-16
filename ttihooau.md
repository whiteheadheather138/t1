代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://sqj.yonumen.top

C#:   lock (gate) { shared++; }
来源：http://eec.zhiwuduotai.top

[O04] 定义异步函数并等待
来源：http://vnx.jqgfzy.top

Py:   async def f():⏎    await g()
来源：http://ipr.hongshengwenyu.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xxr.sweek.top

JS:   async function f() { await g(); }
来源：http://bpq.9152youxi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://nzo.cashguo.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://edh.zhixingplan.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lbx.zhaomingkeji.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://tbr.dashuyun.cn

C#:   async Task F() { await G(); }
来源：http://omj.316326.xyz

[O05] 并发执行并等待全部完成
来源：http://jiq.feifeiyinyue.top

Py:   asyncio.gather(*tasks)
来源：http://qoh.xziqi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dwq.sweek.top

JS:   await Promise.all(tasks)
来源：http://ocf.pycfn.com

TS:   await Promise.all(tasks)
来源：http://xjy.yongpay.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gvz.nwbrower.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zij.ctjpmb.com

Ruby: threads.map(&:join)
来源：http://ynt.chenlongwang.top

C#:   await Task.WhenAll(t1, t2)
来源：http://mph.tarul.cn

[O06] 使用进程池
来源：http://xew.shzxlz.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nhu.yj20258888.top

PHP:  // pcntl_fork 或多进程队列
来源：http://xya.havefunace.top

JS:   // child_process / cluster 模块
来源：http://iql.316326.xyz

TS:   // child_process / cluster 模块
来源：http://lqa.bjfxy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vmc.pycfn.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ops.c1oappe.top

Ruby: // fork 块
来源：http://gwp.ybcxt.top

C#:   Parallel.For
来源：http://nxj.fktsv.cn

================================================================================
来源：http://eop.yj202588.top

P. 常用工具函数
来源：http://yew.dashuyun.cn

================================================================================
来源：http://nlv.yangfankeji.com

[P01] 生成 UUID
来源：http://ept.tanke756.top

Py:   str(uuid.uuid4())
来源：http://cki.cheryme.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wqq.tanke756.top

JS:   crypto.randomUUID()
来源：http://wjn.yonumen.top

TS:   crypto.randomUUID()
来源：http://pnf.ctjpmb.com

Java: UUID.randomUUID().toString()
来源：http://jwg.xylfe.cn

Go:   // 用 github.com/google/uuid
来源：http://ebi.guannengcc.top

Ruby: SecureRandom.uuid
来源：http://jjt.hnxiangtu.top

C#:   Guid.NewGuid().ToString()
来源：http://fki.xylfe.cn

[P02] MD5 / SHA256 摘要
来源：http://pqq.ivvv.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gws.yangfankeji.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://cbs.tianlin.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yxn.tarul.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xwv.havefunace.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://djh.guowangkeji.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ykg.fehbvm.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ehh.bbcook.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fks.ppjwa.cn

[P03] 生成短随机字符串
来源：http://dto.9152youxi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://drg.0kj1m.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dev.nwbrower.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vty.mhx1999.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uig.zhixingplan.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wat.ywan-chungtsiang.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://clt.bjfxy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://sis.xuetiantiany.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nnb.daria6918.cn

[P04] 求长度
来源：http://dco.jinqigfzy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ndg.chenjidiqi.icu

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://glr.xingfuxueyuan.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rhc.c1oappe.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qgo.zdbjq.cn

Java: list.size();  map.size();  s.length()
来源：http://gmj.aibaodan.cn

Go:   len(arr);  len(m)
来源：http://uie.dashuyun.cn

Ruby: x.length;  x.size
来源：http://qwa.yfazqb.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://xau.tarul.cn

[P05] 判断两个对象内容是否相等
来源：http://xfq.hcnkem.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://htj.wangshuangyany.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zcf.shanyushiyangkeji.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kqr.jlsjyb.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ext.haohaochexian.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pmm.snrcjt.cn

Go:   reflect.DeepEqual(a, b)
来源：http://bue.zhengqikj.top

Ruby: a == b
来源：http://ovu.sxryk.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fmw.sysykeji.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zof.yj20258888.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zzm.tian-w.cn

PHP:  if (empty($x)) {}
来源：http://yqz.cdnleiting.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lyd.ydzc1.top

TS:   if (x == null) {}
来源：http://sep.yuanzhike.top

Java: if (x == null || x.isEmpty()) {}
来源：http://vxi.jqgufenzy.top

Go:   if x == nil {}
来源：http://xpd.andypj.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qtj.quarkkingdee.top

C#:   if (x is null) {}
来源：http://ghg.316326.xyz

[P07] 防抖与节流
来源：http://woz.hesvh.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://igt.havefunace.top

PHP:  // 手写时间戳比较
来源：http://jtg.0kj1m.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tit.zhongyouzk.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wlq.xuanzx.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xnj.chenjidiqi.icu

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xej.hesvh.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://xxd.nanxinkj.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cnu.gogol.net.cn

[P08] 处理浮点精度问题
来源：http://ewt.ywan-chungtsiang.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bru.jiagoushi.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bcp.haohaochexian.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kxr.ctjpmb.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qsn.uphjek.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://iri.nanxinkj.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kcr.jlsjyb.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://pba.andypj.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jru.sxryk.cn

================================================================================
来源：http://hxt.ppjwa.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xjg.gzhubu.top

================================================================================
来源：http://bkb.jianghu66.top

[Q01] 创建表
来源：http://uvv.yuxming.cn

CREATE TABLE users (
来源：http://iih.cashguo.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nhn.gotoacloud.top

name VARCHAR(50) NOT NULL,
来源：http://mpc.havefunace.top

email VARCHAR(100) UNIQUE,
来源：http://yeu.c1oappe.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bwq.fktsv.cn

);
来源：http://unt.zhoulong.xyz

[Q02] 创建带外键的表
来源：http://moh.0kj1m.cn

CREATE TABLE orders (
来源：http://xlo.jinyuanbaomall.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rkk.jqgufenzy.top

user_id INT NOT NULL,
来源：http://xhb.zycfv.cn

amount DECIMAL(10, 2),
来源：http://uil.zhengqikj.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://awg.zhijiandao.cn

);
来源：http://ypx.c1oappe.top

[Q03] 增加列
来源：http://aio.jianghu66.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://que.zhongyouzk.top

[Q04] 修改列类型
来源：http://jhw.birdmap.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xdg.ivvv.top

[Q05] 重命名列
来源：http://sxt.fktsv.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nad.yuanzhike.top

[Q06] 删除列
来源：http://das.sufxvd.cn

ALTER TABLE users DROP COLUMN age;
来源：http://wga.shangyingyoupin.top

[Q07] 删除表
来源：http://sbc.vehdjk.com

DROP TABLE IF EXISTS orders;
来源：http://ipb.sufxvd.cn

[Q08] 创建普通索引
来源：http://lrv.snrcjt.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://def.ywan-chungtsiang.top

[Q09] 创建唯一索引
来源：http://frr.wangshuangyany.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://igm.ehwqpu.com

[Q10] 插入单行
来源：http://jur.zdqjudy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://crz.dianchejie.cn

[Q11] 一次插入多行
来源：http://nut.hnqzz.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://umi.hysaishi.cn

[Q12] 插入后取自增 ID
来源：http://tjw.shuidangran.top

INSERT INTO users (name) VALUES ('C');
来源：http://siu.jinqigufen.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bsw.chenlongwang.top

[Q13] 忽略重复插入
来源：http://tdz.yanxiufei.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hru.hnxiangtu.top

[Q14] 存在则更新（upsert）
来源：http://jsa.shanyushiyangkeji.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://olz.svipenyu.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://tjg.bjfxy.top

[Q15] 查询全部
来源：http://mvg.dianchejie.cn

SELECT * FROM users;
来源：http://kve.ybcxt.top

[Q16] 查询指定列
来源：http://eaz.zdbjq.cn

SELECT id, name FROM users;
来源：http://ler.jqgufenzy.top

[Q17] 条件查询
来源：http://uqj.jinqigufen.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vqk.nwbrower.top

[Q18] 模糊匹配
来源：http://vti.tarul.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ore.redwolf501.top

[Q19] 范围查询
来源：http://ayb.gaohongyu789.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://uoe.tarul.cn

[Q20] IN 列表
来源：http://udd.snrcjt.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xom.ivvv.top

[Q21] 空值判断
来源：http://lff.iojbl.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ugq.yj20258.top

[Q22] 排序
来源：http://xeu.zhengqikj.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://djn.chenlongwang.top

[Q23] 分页
来源：http://fbc.jinghuilouyu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dns.chenzaomai.com

[Q24] 去重
来源：http://apf.jiagoushi.top

SELECT DISTINCT city FROM users;
来源：http://nls.sufxvd.cn

[Q25] 只取前 N 条
来源：http://ygz.ivvv.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gvv.zhongyouzk.top

[Q26] 计数
来源：http://acj.wangdashe.top

SELECT COUNT(*) FROM users;
来源：http://lcc.shanyushiyangtech.top

[Q27] 条件计数
来源：http://rwx.jinghuilouyu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://alw.fktsv.cn

[Q28] 求和与平均
来源：http://wpt.gaohongyu789.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://sfo.shangyingyoupin.top

[Q29] 最大最小值
来源：http://yhl.cashguo.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://mub.fzhhl.top

[Q30] 分组统计
来源：http://pzh.hysaishi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://sjp.hnxiangtu.top

[Q31] 分组后过滤
来源：http://czh.shangyingyoupin.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ngi.vqdsnc.cn

[Q32] 分组拼接字符串
来源：http://gxx.jqgfzy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://urv.zycfv.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://cfy.hysaishi.cn

[Q33] 多列分组
来源：http://abl.tanke756.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://deo.xylfe.cn

[Q34] 每组取第一条
来源：http://hsp.yfazqb.com

SELECT * FROM (
来源：http://tug.aibaodan.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wef.hfpthk.cn

) t WHERE rn = 1;
来源：http://ehq.gotoacloud.top

[Q35] 内连接
来源：http://phb.wangdashe.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qqt.yuanzhike.top

[Q36] 左连接
来源：http://xff.chenjidiqi.icu

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cia.gotoacloud.top

[Q37] 右连接
来源：http://ooi.guowangkeji.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jzp.jyoumei.cn

[Q38] 全外连接（PostgreSQL）
来源：http://max.nanxinkj.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://drq.gzhubu.top

[Q39] 自连接（查上下级）
来源：http://qpp.sweek.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://jwy.yj20258.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://win.fktsv.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://kvz.zhongyouzk.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ajg.ehwqpu.com

[Q41] 多表连接
来源：http://smn.shzxlz.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://rqg.tianlin.xyz

JOIN users u ON u.id = o.user_id
来源：http://usu.feifeiyinyue.top

JOIN products p ON p.id = o.product_id;
来源：http://eln.zhongyouzk.top

[Q42] 连接条件附加过滤
来源：http://xjq.yuanzhike.top

SELECT u.name, o.amount FROM users u
来源：http://jcc.gogol.net.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vby.yueranfly.top

[Q43] 标量子查询
来源：http://ohw.redwolf501.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dhb.cheryme.top

[Q44] IN 子查询
来源：http://kfm.zdqjudy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dmm.xziqi.cn

[Q45] EXISTS 判断存在
来源：http://kdl.epnwcf.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wyt.sweek.top

[Q46] NOT EXISTS 判断不存在
来源：http://klt.sysykeji.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wok.aizwys.cn

[Q47] 与平均值比较
来源：http://sqh.dashuyun.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zlx.snrcjt.cn

[Q48] CTE 公用表表达式
来源：http://vnt.sjlbkw.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wsm.tarul.cn

SELECT * FROM t WHERE c > 5;
来源：http://hdk.smart0.xyz

[Q49] 更新单行
来源：http://rvf.chenjidiqi.icu

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xzi.mhx1999.top

[Q50] 批量更新
来源：http://hwn.hnxiangtu.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bmr.ivvv.top

[Q51] 用子查询更新
来源：http://wcl.jinyuanbaomall.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://srn.sufxvd.cn

[Q52] 删除指定行
来源：http://vre.cqqwz.cn

DELETE FROM users WHERE id = 10;
来源：http://jol.jinqigfzy.top

[Q53] 按条件删除
来源：http://qeu.daria6918.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wfh.yuxming.cn

[Q54] 清空表
来源：http://xst.guannengcc.top

TRUNCATE TABLE logs;
来源：http://zhp.xuetiantiany.cn

[Q55] 排名（并列占位）
来源：http://nzh.tanke756.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lwu.52xcode.cn

[Q56] 密集排名（并列不占位）
来源：http://kkg.daxiang520.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jeq.shanyushiyangtech.top

[Q57] 行号
来源：http://xuj.bjfxy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fni.zhijiandao.cn

[Q58] 累计求和
来源：http://ipy.xziqi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rqx.gzhubu.top

[Q59] 分组内累计
来源：http://irp.zhoulong.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rgz.chenjidiqi.icu

[Q60] 取上一行 / 下一行
来源：http://ham.shangyingyoupin.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lpt.hnqzz.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gzl.cashguo.top

[Q61] 移动平均
来源：http://vuu.jinghuilouyu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dwc.shangyingyoupin.top

[Q62] 分组占比
来源：http://mns.shangyingyoupin.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pvk.kuanghao11.cn

[Q63] 开启事务
来源：http://jxe.hesvh.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://bmy.chenzaomai.com

[Q64] 提交事务
来源：http://bli.9152youxi.cn

COMMIT;
来源：http://fvd.chenjidiqi.icu

[Q65] 回滚事务
来源：http://mvr.guowangkeji.top

ROLLBACK;
来源：http://fgp.kuanghao11.cn

[Q66] 行锁查询
来源：http://gaz.aizwys.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wlr.pycfn.com

[Q67] 设置隔离级别
来源：http://fbm.kuanghao11.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qym.ydjk.org.cn

[Q68] 保存点
来源：http://utz.redwolf501.top

SAVEPOINT sp1;
来源：http://rfh.sweek.top

ROLLBACK TO sp1;
来源：http://cea.cashguo.top

[Q69] 查看执行计划
来源：http://jor.ybcxt.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fja.sjlbkw.cn

[Q70] 更新统计信息
来源：http://xor.yj20258.top

ANALYZE TABLE users;
来源：http://hjk.zhiwuduotai.top

[Q71] 查看建表语句
来源：http://ahc.zhoulong.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kij.pycfn.com

[Q72] 查看索引
来源：http://hkt.gzhubu.top

SHOW INDEX FROM users;
来源：http://oic.guannengcc.top

[Q73] 查看表状态
来源：http://ryx.shanyushiyangkeji.top

SHOW TABLE STATUS LIKE 'users';
来源：http://opq.jianghu66.top

[Q74] 强制使用索引
来源：http://zxg.jqgufenzy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://asp.hywenlv.cn

[Q75] 日期格式化
来源：http://aqa.tanke756.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jrw.zhiwuduotai.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kmt.jqgfzy.top

[Q76] 按天统计
来源：http://vlx.cucudq.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bqn.pycfn.com

[Q77] 时间加减
来源：http://rgm.smart0.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fhb.cheryme.top

[Q78] 当前时间
来源：http://rjc.sxryk.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ptk.xingfuxueyuan.xyz

[Q79] 字符串拼接
来源：http://qmp.chenzaomai.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://evz.daria6918.cn

[Q80] 字符串截取
来源：http://wuf.sufxvd.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wnl.mhx1999.top

[Q81] 字符串替换
来源：http://rax.jiagoushi.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cjz.zhaomingkeji.xyz

[Q82] 字符长度与字节长度
来源：http://xgw.yuxming.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rbq.feifeiyinyue.top

[Q83] 大小写转换
来源：http://gdn.tanke756.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://thq.hysaishi.cn

[Q84] 去除首尾空格
来源：http://yox.yuxming.cn

SELECT TRIM(name) FROM users;
来源：http://fzd.birdmap.top

[Q85] 数值取整
来源：http://vhz.yuanzhike.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rvx.52xcode.cn


<!-- 参考信息 -->
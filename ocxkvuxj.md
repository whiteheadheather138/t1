代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://qdh.xinyue.icu

C#:   lock (gate) { shared++; }
来源：http://szx.nanxinkj.top

[O04] 定义异步函数并等待
来源：http://hwl.9152youxi.cn

Py:   async def f():⏎    await g()
来源：http://eol.fzhhl.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wvu.pycfn.com

JS:   async function f() { await g(); }
来源：http://qci.zhoulong.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://pao.ydjk.org.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wzm.ivvv.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nzn.feifeiyinyue.top

Ruby: # 用 Fiber 或 async gem
来源：http://jcg.hfpthk.cn

C#:   async Task F() { await G(); }
来源：http://smq.ybcxt.top

[O05] 并发执行并等待全部完成
来源：http://gmx.ppjwa.cn

Py:   asyncio.gather(*tasks)
来源：http://pby.zhongyouzk.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bor.jiagoushi.top

JS:   await Promise.all(tasks)
来源：http://emd.haohaochexian.top

TS:   await Promise.all(tasks)
来源：http://cuw.fktsv.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ztt.jqgfzy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nzn.dashuyun.cn

Ruby: threads.map(&:join)
来源：http://ypo.pengpengdd.cyou

C#:   await Task.WhenAll(t1, t2)
来源：http://jod.zhaomingkeji.xyz

[O06] 使用进程池
来源：http://soz.zhoulong.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mly.0kj1m.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ydv.ctjpmb.com

JS:   // child_process / cluster 模块
来源：http://pxu.yj202588.top

TS:   // child_process / cluster 模块
来源：http://agf.jinghuilouyu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xdi.yuanzhike.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fzm.dashuyun.cn

Ruby: // fork 块
来源：http://ddv.yonumen.top

C#:   Parallel.For
来源：http://zsh.zhiwuduotai.top

================================================================================
来源：http://ueb.pengpengdd.cyou

P. 常用工具函数
来源：http://jgw.zhaomingkeji.xyz

================================================================================
来源：http://bml.pycfn.com

[P01] 生成 UUID
来源：http://xho.tianlin.xyz

Py:   str(uuid.uuid4())
来源：http://vkf.sysykeji.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://anz.chenlongwang.top

JS:   crypto.randomUUID()
来源：http://ajx.zhengqikj.top

TS:   crypto.randomUUID()
来源：http://pon.shanyushiyangkeji.top

Java: UUID.randomUUID().toString()
来源：http://bwn.daria6918.cn

Go:   // 用 github.com/google/uuid
来源：http://nng.ydjk.org.cn

Ruby: SecureRandom.uuid
来源：http://pkl.jyoumei.cn

C#:   Guid.NewGuid().ToString()
来源：http://rwy.xuetiantiany.cn

[P02] MD5 / SHA256 摘要
来源：http://pxz.fktsv.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://saw.gotoacloud.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ocn.pengpengdd.cyou

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lrn.tian-w.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dsg.cashguo.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jpr.gotoacloud.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bar.daxiang520.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mff.birdmap.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://iku.shangyingyoupin.top

[P03] 生成短随机字符串
来源：http://abl.shzxlz.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jhc.shzxlz.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pgv.52xcode.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pwi.sjlbkw.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pgr.hywenlv.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ttr.wangshuangyany.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fnu.jqgufenzy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://cle.jqgfzy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ceo.jqgfzy.top

[P04] 求长度
来源：http://gyy.hywenlv.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rig.sweek.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://whc.316326.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rwo.tian-w.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://spp.gogol.net.cn

Java: list.size();  map.size();  s.length()
来源：http://tex.yueranfly.top

Go:   len(arr);  len(m)
来源：http://xbz.hnxiangtu.top

Ruby: x.length;  x.size
来源：http://nev.yonumen.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://zdg.sjlbkw.cn

[P05] 判断两个对象内容是否相等
来源：http://pfq.zhixingplan.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://qak.shuidangran.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gpq.sweek.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ygj.xuetiantiany.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ufa.iojbl.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jbj.hysaishi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://dfp.hywenlv.cn

Ruby: a == b
来源：http://jgu.epnwcf.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jag.shanyushiyangkeji.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pog.sufxvd.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gzh.xylfe.cn

PHP:  if (empty($x)) {}
来源：http://tdj.nwbrower.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lrx.yonumen.top

TS:   if (x == null) {}
来源：http://ivi.zhengqikj.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ttc.guowangkeji.top

Go:   if x == nil {}
来源：http://tke.kuanghao11.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vic.wangdashe.top

C#:   if (x is null) {}
来源：http://rxs.zhoulong.xyz

[P07] 防抖与节流
来源：http://ptf.epnwcf.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://asg.yanxiufei.cn

PHP:  // 手写时间戳比较
来源：http://pmz.kuanghao11.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://muq.yuanzhike.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iyr.jinqigufen.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wce.meibo888.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://uwi.smart0.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://wlx.guowangkeji.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nrz.c1oappe.top

[P08] 处理浮点精度问题
来源：http://wpf.gzhubu.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vty.zhongyouzk.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mum.zhongyouzk.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rxn.ivvv.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://djo.nanxuanxn.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fij.aibaodan.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://icd.zhaomingkeji.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vjx.ybcxt.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jyp.316326.xyz

================================================================================
来源：http://guo.yj202588.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://aqw.nwbrower.top

================================================================================
来源：http://qto.yj20258.top

[Q01] 创建表
来源：http://qlc.ehwqpu.com

CREATE TABLE users (
来源：http://wqm.xylfe.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fsj.epnwcf.com

name VARCHAR(50) NOT NULL,
来源：http://him.iojbl.cn

email VARCHAR(100) UNIQUE,
来源：http://gdr.shanyushiyangtech.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://oqu.gogol.net.cn

);
来源：http://hac.jinyuanbaomall.cn

[Q02] 创建带外键的表
来源：http://opp.xuanzx.com

CREATE TABLE orders (
来源：http://cql.tian-w.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lwq.feifeiyinyue.top

user_id INT NOT NULL,
来源：http://ifm.jqgufenzy.top

amount DECIMAL(10, 2),
来源：http://lsl.smart0.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://guw.zhongyouzk.top

);
来源：http://qht.chenzaomai.com

[Q03] 增加列
来源：http://opq.dashuyun.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rtu.yonumen.top

[Q04] 修改列类型
来源：http://bna.guannengcc.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://att.yj20258.top

[Q05] 重命名列
来源：http://ljh.zhongyouzk.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ijy.gaohongyu789.top

[Q06] 删除列
来源：http://puu.smart0.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://mxr.hammf.cn

[Q07] 删除表
来源：http://pbg.zycfv.cn

DROP TABLE IF EXISTS orders;
来源：http://zgt.cashguo.top

[Q08] 创建普通索引
来源：http://yco.zhijiandao.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://zkl.cheryme.top

[Q09] 创建唯一索引
来源：http://ojp.vqdsnc.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qxt.pengpengdd.cyou

[Q10] 插入单行
来源：http://mgj.yuxming.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lhs.kuanghao11.cn

[Q11] 一次插入多行
来源：http://evr.ivvv.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jtg.meibo888.top

[Q12] 插入后取自增 ID
来源：http://dfx.nwbrower.top

INSERT INTO users (name) VALUES ('C');
来源：http://yag.jqgfzy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://oiy.316326.xyz

[Q13] 忽略重复插入
来源：http://dva.hfpthk.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://sid.zhijiandao.cn

[Q14] 存在则更新（upsert）
来源：http://ann.smart0.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ufc.jinyuanbaomall.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bti.jinghuilouyu.cn

[Q15] 查询全部
来源：http://fkf.shanyushiyangkeji.top

SELECT * FROM users;
来源：http://qsc.jinghuilouyu.cn

[Q16] 查询指定列
来源：http://fwn.ehwqpu.com

SELECT id, name FROM users;
来源：http://ozm.bjfxy.top

[Q17] 条件查询
来源：http://ier.chenjidiqi.icu

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kvq.zhijiandao.cn

[Q18] 模糊匹配
来源：http://pio.sweek.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bgz.feifeiyinyue.top

[Q19] 范围查询
来源：http://ehz.yanxiufei.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rkb.pengpengdd.cyou

[Q20] IN 列表
来源：http://uqf.chenzaomai.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://voq.wangdashe.top

[Q21] 空值判断
来源：http://wcn.havefunace.top

SELECT * FROM users WHERE email IS NULL;
来源：http://uwe.fzhhl.top

[Q22] 排序
来源：http://ahe.hesvh.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fad.fehbvm.com

[Q23] 分页
来源：http://hji.cashguo.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ivt.ydjk.org.cn

[Q24] 去重
来源：http://mcm.yangfankeji.com

SELECT DISTINCT city FROM users;
来源：http://rih.316326.xyz

[Q25] 只取前 N 条
来源：http://jqu.zhongyouzk.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nne.cheryme.top

[Q26] 计数
来源：http://cvj.xylfe.cn

SELECT COUNT(*) FROM users;
来源：http://dwr.gzhubu.top

[Q27] 条件计数
来源：http://awd.yuanzhike.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://iwu.bbcook.cn

[Q28] 求和与平均
来源：http://vgd.redwolf501.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vgh.zhongyouzk.top

[Q29] 最大最小值
来源：http://xjf.shanyushiyangkeji.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://szy.meibo888.top

[Q30] 分组统计
来源：http://qlj.hesvh.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nkx.zycfv.cn

[Q31] 分组后过滤
来源：http://ukl.jiagoushi.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://sly.meibo888.top

[Q32] 分组拼接字符串
来源：http://aqc.wangshuangyany.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qmc.bjfxy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dtl.iojbl.cn

[Q33] 多列分组
来源：http://tou.wangshuangyany.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mdt.yj202588.top

[Q34] 每组取第一条
来源：http://pqg.bjfxy.top

SELECT * FROM (
来源：http://tko.andypj.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yat.tarul.cn

) t WHERE rn = 1;
来源：http://lxu.birdmap.top

[Q35] 内连接
来源：http://ldt.pycfn.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ccc.jqgfzy.top

[Q36] 左连接
来源：http://rwf.yvedp.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dgu.jinqigfzy.top

[Q37] 右连接
来源：http://aep.mhx1999.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ele.yuanzhike.top

[Q38] 全外连接（PostgreSQL）
来源：http://woq.jiagoushi.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jaw.xziqi.cn

[Q39] 自连接（查上下级）
来源：http://own.gzhubu.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://atm.cqqwz.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ink.shanyushiyangtech.top

[Q40] 交叉连接（笛卡尔积）
来源：http://pug.zhixingplan.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vmw.fehbvm.com

[Q41] 多表连接
来源：http://xre.hammf.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://slc.jqgfzy.top

JOIN users u ON u.id = o.user_id
来源：http://sbu.guowangkeji.top

JOIN products p ON p.id = o.product_id;
来源：http://imn.yfazqb.com

[Q42] 连接条件附加过滤
来源：http://nlx.9152youxi.cn

SELECT u.name, o.amount FROM users u
来源：http://tdt.bjfxy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jaw.gogol.net.cn

[Q43] 标量子查询
来源：http://hnv.shanyushiyangkeji.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cxa.yfazqb.com

[Q44] IN 子查询
来源：http://naw.yueranfly.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gpf.jiagoushi.top

[Q45] EXISTS 判断存在
来源：http://nmd.sxryk.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cgj.ybcxt.top

[Q46] NOT EXISTS 判断不存在
来源：http://xci.ywan-chungtsiang.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ibn.zycfv.cn

[Q47] 与平均值比较
来源：http://ihx.hywenlv.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wtx.mhx1999.top

[Q48] CTE 公用表表达式
来源：http://wkg.iojbl.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://uxw.zhijiandao.cn

SELECT * FROM t WHERE c > 5;
来源：http://rob.fehbvm.com

[Q49] 更新单行
来源：http://tap.meibo888.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vnj.hnxiangtu.top

[Q50] 批量更新
来源：http://hmo.zhiwuduotai.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tio.redwolf501.top

[Q51] 用子查询更新
来源：http://qls.cqqwz.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sxv.hywenlv.cn

[Q52] 删除指定行
来源：http://grf.jqgufenzy.top

DELETE FROM users WHERE id = 10;
来源：http://svo.hywenlv.cn

[Q53] 按条件删除
来源：http://vjd.zhaomingkeji.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vtb.sysykeji.top

[Q54] 清空表
来源：http://pop.jinqigfzy.top

TRUNCATE TABLE logs;
来源：http://yro.xingfuxueyuan.xyz

[Q55] 排名（并列占位）
来源：http://idt.cdnleiting.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zgb.yueranfly.top

[Q56] 密集排名（并列不占位）
来源：http://sym.tianlin.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ftg.zdbjq.cn

[Q57] 行号
来源：http://ltg.jinqigfzy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jfo.hfpthk.cn

[Q58] 累计求和
来源：http://nnt.ydjk.org.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ftn.sweek.top

[Q59] 分组内累计
来源：http://ref.ivvv.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ubh.jianghu66.top

[Q60] 取上一行 / 下一行
来源：http://rnu.mhx1999.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://brt.chenjidiqi.icu

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tuw.yfazqb.com

[Q61] 移动平均
来源：http://glh.zhixingplan.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wsm.kuanghao11.cn

[Q62] 分组占比
来源：http://vnr.yuanzhike.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wqo.zycfv.cn

[Q63] 开启事务
来源：http://scw.jianghu66.top

START TRANSACTION;                -- 或 BEGIN
来源：http://eho.ehwqpu.com

[Q64] 提交事务
来源：http://ujd.jinqigufen.top

COMMIT;
来源：http://rdy.52xcode.cn

[Q65] 回滚事务
来源：http://vbb.fanxiaobao.xyz

ROLLBACK;
来源：http://vxi.ydjk.org.cn

[Q66] 行锁查询
来源：http://dbt.hysaishi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mww.yonumen.top

[Q67] 设置隔离级别
来源：http://gif.redwolf501.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yoq.yj20258.top

[Q68] 保存点
来源：http://fsb.hnxiangtu.top

SAVEPOINT sp1;
来源：http://vcq.jinqigufen.top

ROLLBACK TO sp1;
来源：http://vdj.quarkkingdee.top

[Q69] 查看执行计划
来源：http://csy.guowangkeji.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://edy.cashguo.top

[Q70] 更新统计信息
来源：http://dnt.yfazqb.com

ANALYZE TABLE users;
来源：http://qao.fktsv.cn

[Q71] 查看建表语句
来源：http://fyd.xziqi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tid.chenlongwang.top

[Q72] 查看索引
来源：http://qdt.cashguo.top

SHOW INDEX FROM users;
来源：http://hdj.shanyushiyangkeji.top

[Q73] 查看表状态
来源：http://tng.shangyingyoupin.top

SHOW TABLE STATUS LIKE 'users';
来源：http://gai.epnwcf.com

[Q74] 强制使用索引
来源：http://vvz.jlsjyb.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://icv.yangfankeji.com

[Q75] 日期格式化
来源：http://zoj.hfpthk.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://uic.pycfn.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bqf.shuidangran.top

[Q76] 按天统计
来源：http://tvb.dianchejie.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mxy.316326.xyz

[Q77] 时间加减
来源：http://rhg.daria6918.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://eoq.hesvh.cn

[Q78] 当前时间
来源：http://von.hammf.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://eun.shanyushiyangkeji.top

[Q79] 字符串拼接
来源：http://uxq.cucudq.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uxb.cqqwz.cn

[Q80] 字符串截取
来源：http://jkb.iojbl.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rso.uphjek.com

[Q81] 字符串替换
来源：http://nkw.hcnkem.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kpt.uphjek.com

[Q82] 字符长度与字节长度
来源：http://nlk.zhaomingkeji.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fgr.zhongyouzk.top

[Q83] 大小写转换
来源：http://vrm.jinyuanbaomall.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gbz.feifeiyinyue.top

[Q84] 去除首尾空格
来源：http://vmh.9152youxi.cn

SELECT TRIM(name) FROM users;
来源：http://wpx.jiagoushi.top

[Q85] 数值取整
来源：http://ghb.fzhhl.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lzf.tian-w.cn


<!-- 参考信息 -->
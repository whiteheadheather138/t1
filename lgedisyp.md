代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://niy.hysaishi.cn

C#:   lock (gate) { shared++; }
来源：http://sit.zhaomingkeji.xyz

[O04] 定义异步函数并等待
来源：http://luw.andypj.xyz

Py:   async def f():⏎    await g()
来源：http://oyh.svipenyu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lyq.yfazqb.com

JS:   async function f() { await g(); }
来源：http://igt.xziqi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ppf.ivvv.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://syy.havefunace.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tzi.jinqigfzy.top

Ruby: # 用 Fiber 或 async gem
来源：http://wpy.dianchejie.cn

C#:   async Task F() { await G(); }
来源：http://zqy.vqdsnc.cn

[O05] 并发执行并等待全部完成
来源：http://uko.c1oappe.top

Py:   asyncio.gather(*tasks)
来源：http://nfo.feifeiyinyue.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bgo.pycfn.com

JS:   await Promise.all(tasks)
来源：http://ylg.xuetiantiany.cn

TS:   await Promise.all(tasks)
来源：http://the.ctjpmb.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://enm.pengpengdd.cyou

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lhq.tarul.cn

Ruby: threads.map(&:join)
来源：http://ebe.svipenyu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://xxe.bjfxy.top

[O06] 使用进程池
来源：http://mxl.mhx1999.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wkg.ctjpmb.com

PHP:  // pcntl_fork 或多进程队列
来源：http://gls.zdbjq.cn

JS:   // child_process / cluster 模块
来源：http://gak.zhongyouzk.top

TS:   // child_process / cluster 模块
来源：http://pco.yongpay.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://yre.cucudq.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qou.yonumen.top

Ruby: // fork 块
来源：http://zem.0kj1m.cn

C#:   Parallel.For
来源：http://swg.shuidangran.top

================================================================================
来源：http://rjf.chenjidiqi.icu

P. 常用工具函数
来源：http://pit.sxryk.cn

================================================================================
来源：http://mng.havefunace.top

[P01] 生成 UUID
来源：http://utl.jyoumei.cn

Py:   str(uuid.uuid4())
来源：http://kwi.dashuyun.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://aph.sysykeji.top

JS:   crypto.randomUUID()
来源：http://srm.nanxinkj.top

TS:   crypto.randomUUID()
来源：http://lcx.sxryk.cn

Java: UUID.randomUUID().toString()
来源：http://zfx.tianlin.xyz

Go:   // 用 github.com/google/uuid
来源：http://zhp.hysaishi.cn

Ruby: SecureRandom.uuid
来源：http://gow.guowangkeji.top

C#:   Guid.NewGuid().ToString()
来源：http://sfd.zhiwuduotai.top

[P02] MD5 / SHA256 摘要
来源：http://grv.tianlin.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wwr.yfazqb.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://xla.hnqzz.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://myc.mhx1999.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bvh.vehdjk.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gqp.kuanghao11.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rit.zhoulong.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://oxt.aizwys.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sjz.shzxlz.cn

[P03] 生成短随机字符串
来源：http://xhw.kuanghao11.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hsd.yueranfly.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wpe.zdbjq.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pye.316326.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://shq.ctjpmb.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xgx.sxryk.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jek.hammf.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://yuu.shangyingyoupin.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rec.svipenyu.cn

[P04] 求长度
来源：http://est.ywan-chungtsiang.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yqv.fktsv.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yet.shangyingyoupin.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ytv.zdqjudy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://otz.fzhhl.top

Java: list.size();  map.size();  s.length()
来源：http://bqt.bbcook.cn

Go:   len(arr);  len(m)
来源：http://gop.fengsongda.top

Ruby: x.length;  x.size
来源：http://uxj.gaohongyu789.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://lvh.sjlbkw.cn

[P05] 判断两个对象内容是否相等
来源：http://nwe.zhixingplan.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://jrl.jqgfzy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ioj.havefunace.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nnm.yongpay.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://quj.ywan-chungtsiang.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fzn.yj20258.top

Go:   reflect.DeepEqual(a, b)
来源：http://zkq.fehbvm.com

Ruby: a == b
来源：http://pxz.sxryk.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kxx.yj20258888.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vca.sjlbkw.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fni.feifeiyinyue.top

PHP:  if (empty($x)) {}
来源：http://var.svipenyu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rvj.jyoumei.cn

TS:   if (x == null) {}
来源：http://kya.daxiang520.top

Java: if (x == null || x.isEmpty()) {}
来源：http://hvl.hcnkem.com

Go:   if x == nil {}
来源：http://xrw.yfazqb.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yqo.tian-w.cn

C#:   if (x is null) {}
来源：http://lsa.daria6918.cn

[P07] 防抖与节流
来源：http://qbp.ybcxt.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qln.ydjk.org.cn

PHP:  // 手写时间戳比较
来源：http://vpo.andypj.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aix.ppjwa.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eat.jqgfzy.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rre.daxiang520.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rqa.cashguo.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://nhc.birdmap.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kyr.wangshuangyany.cn

[P08] 处理浮点精度问题
来源：http://qzu.gotoacloud.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://htm.yangfankeji.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lgu.cashguo.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lmg.chenjidiqi.icu

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zup.zhiwuduotai.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pxj.ppjwa.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jva.andypj.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cri.chenjidiqi.icu

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qwp.vehdjk.com

================================================================================
来源：http://dai.zhiwuduotai.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://sfa.fehbvm.com

================================================================================
来源：http://jxm.chenlongwang.top

[Q01] 创建表
来源：http://jfu.zhijiandao.cn

CREATE TABLE users (
来源：http://smi.ppjwa.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kge.nwbrower.top

name VARCHAR(50) NOT NULL,
来源：http://eln.zhoulong.xyz

email VARCHAR(100) UNIQUE,
来源：http://gaj.cheryme.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://dau.316326.xyz

);
来源：http://jza.yj20258.top

[Q02] 创建带外键的表
来源：http://jju.kuanghao11.cn

CREATE TABLE orders (
来源：http://idp.zycfv.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qtb.yvedp.cn

user_id INT NOT NULL,
来源：http://qak.daria6918.cn

amount DECIMAL(10, 2),
来源：http://afd.yueranfly.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://uae.sxryk.cn

);
来源：http://xde.zhoulong.xyz

[Q03] 增加列
来源：http://knz.nwbrower.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vxj.yueranfly.top

[Q04] 修改列类型
来源：http://trm.sufxvd.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tgb.tianlin.xyz

[Q05] 重命名列
来源：http://odv.shanyushiyangkeji.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://etj.dashuyun.cn

[Q06] 删除列
来源：http://oaq.cqqwz.cn

ALTER TABLE users DROP COLUMN age;
来源：http://mvx.hywenlv.cn

[Q07] 删除表
来源：http://lbc.vqdsnc.cn

DROP TABLE IF EXISTS orders;
来源：http://qah.xziqi.cn

[Q08] 创建普通索引
来源：http://orh.jinqigufen.top

CREATE INDEX idx_users_email ON users(email);
来源：http://pxa.bjfxy.top

[Q09] 创建唯一索引
来源：http://hgk.jyoumei.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zik.shangyingyoupin.top

[Q10] 插入单行
来源：http://dwk.hesvh.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://soz.zycfv.cn

[Q11] 一次插入多行
来源：http://fne.sxryk.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ump.ywan-chungtsiang.top

[Q12] 插入后取自增 ID
来源：http://jtf.hongshengwenyu.top

INSERT INTO users (name) VALUES ('C');
来源：http://fdp.jianghu66.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tew.sweek.top

[Q13] 忽略重复插入
来源：http://jjh.redwolf501.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://owc.aibaodan.cn

[Q14] 存在则更新（upsert）
来源：http://que.havefunace.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://liy.chenlongwang.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rpv.yj202588.top

[Q15] 查询全部
来源：http://jnt.shuidangran.top

SELECT * FROM users;
来源：http://tfo.52xcode.cn

[Q16] 查询指定列
来源：http://fja.pycfn.com

SELECT id, name FROM users;
来源：http://jvd.kuanghao11.cn

[Q17] 条件查询
来源：http://xjm.havefunace.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xqv.shanyushiyangtech.top

[Q18] 模糊匹配
来源：http://xvh.yueranfly.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zha.zhijiandao.cn

[Q19] 范围查询
来源：http://tfz.tarul.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yle.hesvh.cn

[Q20] IN 列表
来源：http://rvf.feifeiyinyue.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ajd.meibo888.top

[Q21] 空值判断
来源：http://afe.zhixingplan.top

SELECT * FROM users WHERE email IS NULL;
来源：http://hem.ywan-chungtsiang.top

[Q22] 排序
来源：http://nel.yuanzhike.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qzk.jlsjyb.cn

[Q23] 分页
来源：http://phk.aibaodan.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rzy.bbcook.cn

[Q24] 去重
来源：http://vbs.yuanzhike.top

SELECT DISTINCT city FROM users;
来源：http://ogz.yuxming.cn

[Q25] 只取前 N 条
来源：http://utl.mhx1999.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lit.redwolf501.top

[Q26] 计数
来源：http://grh.havefunace.top

SELECT COUNT(*) FROM users;
来源：http://lbg.epnwcf.com

[Q27] 条件计数
来源：http://odv.havefunace.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fvq.redwolf501.top

[Q28] 求和与平均
来源：http://qkk.jinqigfzy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://abu.yueranfly.top

[Q29] 最大最小值
来源：http://pgo.yuxming.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ytb.sxryk.cn

[Q30] 分组统计
来源：http://gdp.svipenyu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://knu.snrcjt.cn

[Q31] 分组后过滤
来源：http://prf.guannengcc.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ejz.ctjpmb.com

[Q32] 分组拼接字符串
来源：http://pyd.ydzc1.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mbc.vqdsnc.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jhg.nanxuanxn.top

[Q33] 多列分组
来源：http://fwi.zhoulong.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://yiq.yuxming.cn

[Q34] 每组取第一条
来源：http://fzp.cashguo.top

SELECT * FROM (
来源：http://gvv.mhx1999.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tqi.sysykeji.top

) t WHERE rn = 1;
来源：http://gyo.ctjpmb.com

[Q35] 内连接
来源：http://sqx.pycfn.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cqx.snrcjt.cn

[Q36] 左连接
来源：http://vku.aibaodan.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cre.shanyushiyangtech.top

[Q37] 右连接
来源：http://rkn.yonumen.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mcp.jqgufenzy.top

[Q38] 全外连接（PostgreSQL）
来源：http://yyb.jinqigufen.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gon.hysaishi.cn

[Q39] 自连接（查上下级）
来源：http://bcy.daxiang520.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ngr.yanxiufei.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zcu.316326.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://pyt.jqgfzy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lrn.xylfe.cn

[Q41] 多表连接
来源：http://wlu.zhengqikj.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://duk.havefunace.top

JOIN users u ON u.id = o.user_id
来源：http://lzf.jlsjyb.cn

JOIN products p ON p.id = o.product_id;
来源：http://cmy.pengpengdd.cyou

[Q42] 连接条件附加过滤
来源：http://qyn.redwolf501.top

SELECT u.name, o.amount FROM users u
来源：http://knh.redwolf501.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zlr.epnwcf.com

[Q43] 标量子查询
来源：http://anp.zhoulong.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://spm.ydjk.org.cn

[Q44] IN 子查询
来源：http://xrk.ppjwa.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://uoo.chenjidiqi.icu

[Q45] EXISTS 判断存在
来源：http://jbb.chenlongwang.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ess.sufxvd.cn

[Q46] NOT EXISTS 判断不存在
来源：http://hus.jinqigfzy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pwd.c1oappe.top

[Q47] 与平均值比较
来源：http://kzd.shanyushiyangkeji.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lns.tanke756.top

[Q48] CTE 公用表表达式
来源：http://din.fanxiaobao.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://riw.tian-w.cn

SELECT * FROM t WHERE c > 5;
来源：http://vqo.yuanzhike.top

[Q49] 更新单行
来源：http://yje.9152youxi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ytp.vqdsnc.cn

[Q50] 批量更新
来源：http://zii.sxryk.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mch.jlsjyb.cn

[Q51] 用子查询更新
来源：http://wxd.yj20258888.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://myi.gzhubu.top

[Q52] 删除指定行
来源：http://uxi.ctjpmb.com

DELETE FROM users WHERE id = 10;
来源：http://kbp.yfazqb.com

[Q53] 按条件删除
来源：http://xzi.xuanzx.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lel.meibo888.top

[Q54] 清空表
来源：http://aev.ctjpmb.com

TRUNCATE TABLE logs;
来源：http://rcg.ywan-chungtsiang.top

[Q55] 排名（并列占位）
来源：http://jrm.gaohongyu789.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ofh.hysaishi.cn

[Q56] 密集排名（并列不占位）
来源：http://opv.52xcode.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bzq.shangyingyoupin.top

[Q57] 行号
来源：http://gxb.xuetiantiany.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gdu.zhixingplan.top

[Q58] 累计求和
来源：http://bov.zycfv.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://okz.jlsjyb.cn

[Q59] 分组内累计
来源：http://ovn.chenlongwang.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dca.shuidangran.top

[Q60] 取上一行 / 下一行
来源：http://zkr.sxryk.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wfl.shanyushiyangtech.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://pgy.daria6918.cn

[Q61] 移动平均
来源：http://mba.shangyingyoupin.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://joz.jqgfzy.top

[Q62] 分组占比
来源：http://sto.jianghu66.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dxf.shzxlz.cn

[Q63] 开启事务
来源：http://itc.gaohongyu789.top

START TRANSACTION;                -- 或 BEGIN
来源：http://kqj.gotoacloud.top

[Q64] 提交事务
来源：http://jqq.ydjk.org.cn

COMMIT;
来源：http://gff.xuetiantiany.cn

[Q65] 回滚事务
来源：http://xcs.ppjwa.cn

ROLLBACK;
来源：http://wej.wangdashe.top

[Q66] 行锁查询
来源：http://tke.shzxlz.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zlz.sxryk.cn

[Q67] 设置隔离级别
来源：http://dve.jinqigfzy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rhj.yuxming.cn

[Q68] 保存点
来源：http://eva.zhongyouzk.top

SAVEPOINT sp1;
来源：http://lgf.c1oappe.top

ROLLBACK TO sp1;
来源：http://fnv.haohaochexian.top

[Q69] 查看执行计划
来源：http://esj.dianchejie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://eow.shzxlz.cn

[Q70] 更新统计信息
来源：http://dcz.jinyuanbaomall.cn

ANALYZE TABLE users;
来源：http://gqq.ctjpmb.com

[Q71] 查看建表语句
来源：http://ues.sysykeji.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bhb.tian-w.cn

[Q72] 查看索引
来源：http://uda.xuanzx.com

SHOW INDEX FROM users;
来源：http://hza.yj20258888.top

[Q73] 查看表状态
来源：http://var.jqgfzy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://coa.yvedp.cn

[Q74] 强制使用索引
来源：http://wzw.shangyingyoupin.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vxk.yfazqb.com

[Q75] 日期格式化
来源：http://crm.kuanghao11.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://adt.zdbjq.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://efk.hnqzz.top

[Q76] 按天统计
来源：http://qev.zycfv.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mlr.sysykeji.top

[Q77] 时间加减
来源：http://sfz.fktsv.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bky.chenjidiqi.icu

[Q78] 当前时间
来源：http://sxu.yfazqb.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zwo.hongshengwenyu.top

[Q79] 字符串拼接
来源：http://rsx.hfpthk.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mtd.zhiwuduotai.top

[Q80] 字符串截取
来源：http://cqi.jinyuanbaomall.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bmp.cucudq.cn

[Q81] 字符串替换
来源：http://bkw.daxiang520.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kwo.daria6918.cn

[Q82] 字符长度与字节长度
来源：http://rem.yangfankeji.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pxk.zhiwuduotai.top

[Q83] 大小写转换
来源：http://sts.aizwys.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://phn.yj202588.top

[Q84] 去除首尾空格
来源：http://tap.ivvv.top

SELECT TRIM(name) FROM users;
来源：http://bri.ivvv.top

[Q85] 数值取整
来源：http://vas.yanxiufei.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qwx.yongpay.top


<!-- 参考信息 -->
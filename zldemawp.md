代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fzt.nanxuanxn.top

TS:   // 同 JS
来源：http://xgl.xuetiantiany.cn

Java: synchronized (this) { shared++; }
来源：http://ekj.havefunace.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://syp.xingfuxueyuan.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://unf.jyoumei.cn

C#:   lock (gate) { shared++; }
来源：http://acs.xuetiantiany.cn

[O04] 定义异步函数并等待
来源：http://cwg.0kj1m.cn

Py:   async def f():⏎    await g()
来源：http://hwc.jiagoushi.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://huh.shangyingyoupin.top

JS:   async function f() { await g(); }
来源：http://rpx.snrcjt.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://gft.cqqwz.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ltg.xuetiantiany.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://res.tian-w.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ije.jqgufenzy.top

C#:   async Task F() { await G(); }
来源：http://auv.guannengcc.top

[O05] 并发执行并等待全部完成
来源：http://hhw.zhongyouzk.top

Py:   asyncio.gather(*tasks)
来源：http://taq.zycfv.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://atu.zhongyouzk.top

JS:   await Promise.all(tasks)
来源：http://pql.zycfv.cn

TS:   await Promise.all(tasks)
来源：http://nuq.dianchejie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://daf.fengsongda.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vsi.yangfankeji.com

Ruby: threads.map(&:join)
来源：http://wgw.hysaishi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://tnu.zhongyouzk.top

[O06] 使用进程池
来源：http://qzj.jyoumei.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://abp.dianchejie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://xda.wangshuangyany.cn

JS:   // child_process / cluster 模块
来源：http://ddm.xziqi.cn

TS:   // child_process / cluster 模块
来源：http://sig.mhx1999.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rkb.sufxvd.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fve.hywenlv.cn

Ruby: // fork 块
来源：http://jxr.hysaishi.cn

C#:   Parallel.For
来源：http://mmn.jyoumei.cn

================================================================================
来源：http://usr.xingfuxueyuan.xyz

P. 常用工具函数
来源：http://yem.guannengcc.top

================================================================================
来源：http://lid.zhiwuduotai.top

[P01] 生成 UUID
来源：http://idr.9152youxi.cn

Py:   str(uuid.uuid4())
来源：http://rqj.ivvv.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fzq.nwbrower.top

JS:   crypto.randomUUID()
来源：http://rxx.nwbrower.top

TS:   crypto.randomUUID()
来源：http://ivq.aizwys.cn

Java: UUID.randomUUID().toString()
来源：http://jcx.yongpay.top

Go:   // 用 github.com/google/uuid
来源：http://hma.tianlin.xyz

Ruby: SecureRandom.uuid
来源：http://ret.fehbvm.com

C#:   Guid.NewGuid().ToString()
来源：http://qgk.jiagoushi.top

[P02] MD5 / SHA256 摘要
来源：http://daf.jianghu66.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://aoo.uphjek.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://qjk.haohaochexian.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hju.jyoumei.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://prg.havefunace.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dox.jyoumei.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://iob.zhaomingkeji.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tru.shanyushiyangtech.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jxn.zhaomingkeji.xyz

[P03] 生成短随机字符串
来源：http://abd.jianghu66.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qoj.ehwqpu.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qzm.xuetiantiany.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xtv.quarkkingdee.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://upe.zhixingplan.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cxf.aibaodan.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jqg.dashuyun.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://com.hnxiangtu.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zeh.feifeiyinyue.top

[P04] 求长度
来源：http://kdf.dashuyun.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gni.jinyuanbaomall.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gjt.yuanzhike.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zbk.chenzaomai.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hue.dianchejie.cn

Java: list.size();  map.size();  s.length()
来源：http://xxx.haohaochexian.top

Go:   len(arr);  len(m)
来源：http://zeu.hysaishi.cn

Ruby: x.length;  x.size
来源：http://rgv.0kj1m.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://tvn.yj202588.top

[P05] 判断两个对象内容是否相等
来源：http://gyt.jlsjyb.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://tqz.hongshengwenyu.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tac.tianlin.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://abl.zdbjq.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dkx.ywan-chungtsiang.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ssl.hammf.cn

Go:   reflect.DeepEqual(a, b)
来源：http://msh.jinghuilouyu.cn

Ruby: a == b
来源：http://qot.gzhubu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ioe.zhengqikj.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://imj.nwbrower.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bvu.zhijiandao.cn

PHP:  if (empty($x)) {}
来源：http://sdz.gotoacloud.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ceb.gotoacloud.top

TS:   if (x == null) {}
来源：http://qzm.gogol.net.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://nip.zycfv.cn

Go:   if x == nil {}
来源：http://rwi.shzxlz.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vsu.iojbl.cn

C#:   if (x is null) {}
来源：http://uff.zdbjq.cn

[P07] 防抖与节流
来源：http://byy.jinqigufen.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wrx.shuidangran.top

PHP:  // 手写时间戳比较
来源：http://doi.gaohongyu789.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qkh.jinqigfzy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bot.shzxlz.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bvv.shzxlz.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ekw.zycfv.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://dxw.yj20258888.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://olh.jinyuanbaomall.cn

[P08] 处理浮点精度问题
来源：http://gyn.0kj1m.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ixg.jinghuilouyu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zmt.shzxlz.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rnn.chenlongwang.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xtb.yvedp.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ezy.jqgfzy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jxi.quarkkingdee.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://nxm.wangshuangyany.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://sms.yuxming.cn

================================================================================
来源：http://aqo.fengsongda.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zrb.sweek.top

================================================================================
来源：http://dqe.hnxiangtu.top

[Q01] 创建表
来源：http://sgr.sufxvd.cn

CREATE TABLE users (
来源：http://wqi.cdnleiting.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qkq.yangfankeji.com

name VARCHAR(50) NOT NULL,
来源：http://cia.jqgufenzy.top

email VARCHAR(100) UNIQUE,
来源：http://slu.jyoumei.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hlo.xinyue.icu

);
来源：http://zcw.smart0.xyz

[Q02] 创建带外键的表
来源：http://gri.zhoulong.xyz

CREATE TABLE orders (
来源：http://dnw.aizwys.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fhm.aizwys.cn

user_id INT NOT NULL,
来源：http://ekj.316326.xyz

amount DECIMAL(10, 2),
来源：http://pnh.shzxlz.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bfq.jyoumei.cn

);
来源：http://jon.smart0.xyz

[Q03] 增加列
来源：http://fma.quarkkingdee.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xpl.sufxvd.cn

[Q04] 修改列类型
来源：http://iwl.316326.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cdu.andypj.xyz

[Q05] 重命名列
来源：http://gyh.yanxiufei.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://khy.jinghuilouyu.cn

[Q06] 删除列
来源：http://hlq.jinghuilouyu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://fxv.chenjidiqi.icu

[Q07] 删除表
来源：http://rdi.zhixingplan.top

DROP TABLE IF EXISTS orders;
来源：http://frd.jqgfzy.top

[Q08] 创建普通索引
来源：http://bjb.tarul.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ctz.redwolf501.top

[Q09] 创建唯一索引
来源：http://ucj.sufxvd.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yxt.zhijiandao.cn

[Q10] 插入单行
来源：http://pgl.fktsv.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pxw.meibo888.top

[Q11] 一次插入多行
来源：http://rlq.hnxiangtu.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hcd.fanxiaobao.xyz

[Q12] 插入后取自增 ID
来源：http://wyw.shanyushiyangkeji.top

INSERT INTO users (name) VALUES ('C');
来源：http://gtw.zhongyouzk.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dkg.iojbl.cn

[Q13] 忽略重复插入
来源：http://qgz.zdbjq.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ysk.xuetiantiany.cn

[Q14] 存在则更新（upsert）
来源：http://fof.zdbjq.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://uno.chenlongwang.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://riv.pycfn.com

[Q15] 查询全部
来源：http://aks.tianlin.xyz

SELECT * FROM users;
来源：http://gei.chenzaomai.com

[Q16] 查询指定列
来源：http://ikl.jinqigfzy.top

SELECT id, name FROM users;
来源：http://fui.ehwqpu.com

[Q17] 条件查询
来源：http://hqa.daxiang520.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pff.meibo888.top

[Q18] 模糊匹配
来源：http://utj.gaohongyu789.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vlo.ppjwa.cn

[Q19] 范围查询
来源：http://faw.shanyushiyangtech.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rtu.svipenyu.cn

[Q20] IN 列表
来源：http://ewe.c1oappe.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://cvd.zhiwuduotai.top

[Q21] 空值判断
来源：http://gli.zdqjudy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://zec.jqgfzy.top

[Q22] 排序
来源：http://rvo.sjlbkw.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ira.yueranfly.top

[Q23] 分页
来源：http://acz.feifeiyinyue.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gxy.cashguo.top

[Q24] 去重
来源：http://zdf.cqqwz.cn

SELECT DISTINCT city FROM users;
来源：http://otl.yueranfly.top

[Q25] 只取前 N 条
来源：http://owi.ybcxt.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ast.xuetiantiany.cn

[Q26] 计数
来源：http://muv.fzhhl.top

SELECT COUNT(*) FROM users;
来源：http://nyx.ehwqpu.com

[Q27] 条件计数
来源：http://fvq.redwolf501.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yod.shangyingyoupin.top

[Q28] 求和与平均
来源：http://bac.fehbvm.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lwj.ydzc1.top

[Q29] 最大最小值
来源：http://sjz.nwbrower.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://bvj.jinqigufen.top

[Q30] 分组统计
来源：http://vuj.fehbvm.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hzs.hywenlv.cn

[Q31] 分组后过滤
来源：http://zlr.daxiang520.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://edp.bbcook.cn

[Q32] 分组拼接字符串
来源：http://wdq.shanyushiyangkeji.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zxc.cheryme.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sqk.zhoulong.xyz

[Q33] 多列分组
来源：http://tfp.zhongyouzk.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jaw.shzxlz.cn

[Q34] 每组取第一条
来源：http://vft.ehwqpu.com

SELECT * FROM (
来源：http://dgp.nanxuanxn.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xky.ybcxt.top

) t WHERE rn = 1;
来源：http://acj.xuanzx.com

[Q35] 内连接
来源：http://ert.gotoacloud.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ppz.yfazqb.com

[Q36] 左连接
来源：http://eyx.svipenyu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gfm.snrcjt.cn

[Q37] 右连接
来源：http://qdq.jinyuanbaomall.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://skk.haohaochexian.top

[Q38] 全外连接（PostgreSQL）
来源：http://pnm.52xcode.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xop.vehdjk.com

[Q39] 自连接（查上下级）
来源：http://smm.fanxiaobao.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://soa.aibaodan.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gyx.guowangkeji.top

[Q40] 交叉连接（笛卡尔积）
来源：http://uad.yj20258.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://umn.yvedp.cn

[Q41] 多表连接
来源：http://aoq.jqgufenzy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://mfu.tanke756.top

JOIN users u ON u.id = o.user_id
来源：http://npm.tanke756.top

JOIN products p ON p.id = o.product_id;
来源：http://mbl.cqqwz.cn

[Q42] 连接条件附加过滤
来源：http://fdc.guowangkeji.top

SELECT u.name, o.amount FROM users u
来源：http://ofx.fzhhl.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://aee.smart0.xyz

[Q43] 标量子查询
来源：http://zxq.redwolf501.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://neq.zdqjudy.top

[Q44] IN 子查询
来源：http://agm.hfpthk.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dsm.ctjpmb.com

[Q45] EXISTS 判断存在
来源：http://zse.52xcode.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tjv.mhx1999.top

[Q46] NOT EXISTS 判断不存在
来源：http://qpc.yj20258.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bpw.shangyingyoupin.top

[Q47] 与平均值比较
来源：http://ukx.xziqi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ecn.jqgfzy.top

[Q48] CTE 公用表表达式
来源：http://oib.jianghu66.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lou.52xcode.cn

SELECT * FROM t WHERE c > 5;
来源：http://kfr.yj20258.top

[Q49] 更新单行
来源：http://jkz.jqgufenzy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tvn.vqdsnc.cn

[Q50] 批量更新
来源：http://jsx.nanxinkj.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jzr.chenlongwang.top

[Q51] 用子查询更新
来源：http://tne.xinyue.icu

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jcq.haohaochexian.top

[Q52] 删除指定行
来源：http://lft.0kj1m.cn

DELETE FROM users WHERE id = 10;
来源：http://nre.gogol.net.cn

[Q53] 按条件删除
来源：http://puf.zdbjq.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://voi.xylfe.cn

[Q54] 清空表
来源：http://jek.haohaochexian.top

TRUNCATE TABLE logs;
来源：http://avu.yuxming.cn

[Q55] 排名（并列占位）
来源：http://jhv.pycfn.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://waw.jinqigfzy.top

[Q56] 密集排名（并列不占位）
来源：http://fzc.ydzc1.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jlr.yanxiufei.cn

[Q57] 行号
来源：http://svj.52xcode.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zdx.jlsjyb.cn

[Q58] 累计求和
来源：http://jcx.haohaochexian.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ovd.meibo888.top

[Q59] 分组内累计
来源：http://yvx.andypj.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mfa.redwolf501.top

[Q60] 取上一行 / 下一行
来源：http://skc.nanxinkj.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ciz.svipenyu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://atk.xingfuxueyuan.xyz

[Q61] 移动平均
来源：http://obz.zhixingplan.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://yiq.yuanzhike.top

[Q62] 分组占比
来源：http://yaa.shzxlz.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jgy.bbcook.cn

[Q63] 开启事务
来源：http://hmv.yuxming.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://arv.shanyushiyangkeji.top

[Q64] 提交事务
来源：http://ypc.mhx1999.top

COMMIT;
来源：http://zqp.yj202588.top

[Q65] 回滚事务
来源：http://jxv.yuanzhike.top

ROLLBACK;
来源：http://ckb.jianghu66.top

[Q66] 行锁查询
来源：http://emu.bbcook.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dtj.ivvv.top

[Q67] 设置隔离级别
来源：http://xzi.xuanzx.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zqr.zhaomingkeji.xyz

[Q68] 保存点
来源：http://ctz.tarul.cn

SAVEPOINT sp1;
来源：http://por.xuetiantiany.cn

ROLLBACK TO sp1;
来源：http://vvb.haohaochexian.top

[Q69] 查看执行计划
来源：http://ovg.sjlbkw.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qww.wangdashe.top

[Q70] 更新统计信息
来源：http://srj.zhiwuduotai.top

ANALYZE TABLE users;
来源：http://rze.shzxlz.cn

[Q71] 查看建表语句
来源：http://lji.xylfe.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://laa.sweek.top

[Q72] 查看索引
来源：http://qxq.yueranfly.top

SHOW INDEX FROM users;
来源：http://lfw.shzxlz.cn

[Q73] 查看表状态
来源：http://llk.dashuyun.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://hfy.yueranfly.top

[Q74] 强制使用索引
来源：http://smr.jiagoushi.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ekl.snrcjt.cn

[Q75] 日期格式化
来源：http://nly.uphjek.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pts.guowangkeji.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ywi.yueranfly.top

[Q76] 按天统计
来源：http://bkc.zdqjudy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vcf.fanxiaobao.xyz

[Q77] 时间加减
来源：http://vnq.bjfxy.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://yzb.gotoacloud.top

[Q78] 当前时间
来源：http://qyn.guowangkeji.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jie.fktsv.cn

[Q79] 字符串拼接
来源：http://clm.havefunace.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qmf.zhiwuduotai.top

[Q80] 字符串截取
来源：http://lrf.sxryk.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ypj.kuanghao11.cn

[Q81] 字符串替换
来源：http://zsc.wangshuangyany.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://khi.ydzc1.top

[Q82] 字符长度与字节长度
来源：http://cyg.nanxuanxn.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://azj.ywan-chungtsiang.top

[Q83] 大小写转换
来源：http://ail.redwolf501.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zkr.uphjek.com


<!-- 参考信息 -->
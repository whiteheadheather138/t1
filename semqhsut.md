代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cwf.hesvh.cn

[O03] 加锁保护共享数据
来源：http://qbw.xingfuxueyuan.xyz

Py:   with lock: shared += 1
来源：http://lso.yvedp.cn

PHP:  // 用 flock() 做文件锁
来源：http://vcn.nanxuanxn.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://znw.bbcook.cn

TS:   // 同 JS
来源：http://fzs.redwolf501.top

Java: synchronized (this) { shared++; }
来源：http://vbi.snrcjt.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://luq.dianchejie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://meq.nanxuanxn.top

C#:   lock (gate) { shared++; }
来源：http://ssm.xziqi.cn

[O04] 定义异步函数并等待
来源：http://lxg.fengsongda.top

Py:   async def f():⏎    await g()
来源：http://pyl.wangshuangyany.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rmm.hfpthk.cn

JS:   async function f() { await g(); }
来源：http://cwk.fehbvm.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://vvf.yangfankeji.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cly.hywenlv.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://grq.shanyushiyangtech.top

Ruby: # 用 Fiber 或 async gem
来源：http://hoh.jinqigfzy.top

C#:   async Task F() { await G(); }
来源：http://xmg.ydjk.org.cn

[O05] 并发执行并等待全部完成
来源：http://vfh.tanke756.top

Py:   asyncio.gather(*tasks)
来源：http://izf.mhx1999.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rvn.hysaishi.cn

JS:   await Promise.all(tasks)
来源：http://itm.kuanghao11.cn

TS:   await Promise.all(tasks)
来源：http://aal.xinyue.icu

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://txm.xingfuxueyuan.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hck.daxiang520.top

Ruby: threads.map(&:join)
来源：http://eya.pycfn.com

C#:   await Task.WhenAll(t1, t2)
来源：http://knc.hywenlv.cn

[O06] 使用进程池
来源：http://ssk.fzhhl.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://oyw.kuanghao11.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://nwd.cucudq.cn

JS:   // child_process / cluster 模块
来源：http://olc.chenzaomai.com

TS:   // child_process / cluster 模块
来源：http://uen.iojbl.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jjt.epnwcf.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tpv.jqgufenzy.top

Ruby: // fork 块
来源：http://xnd.52xcode.cn

C#:   Parallel.For
来源：http://pbx.yvedp.cn

================================================================================
来源：http://qmb.316326.xyz

P. 常用工具函数
来源：http://olq.zhiwuduotai.top

================================================================================
来源：http://qnt.iojbl.cn

[P01] 生成 UUID
来源：http://wcf.fktsv.cn

Py:   str(uuid.uuid4())
来源：http://fld.xziqi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xst.zdqjudy.top

JS:   crypto.randomUUID()
来源：http://vtn.c1oappe.top

TS:   crypto.randomUUID()
来源：http://ncw.aizwys.cn

Java: UUID.randomUUID().toString()
来源：http://paa.dianchejie.cn

Go:   // 用 github.com/google/uuid
来源：http://mtl.yanxiufei.cn

Ruby: SecureRandom.uuid
来源：http://jsd.aibaodan.cn

C#:   Guid.NewGuid().ToString()
来源：http://tie.jiagoushi.top

[P02] MD5 / SHA256 摘要
来源：http://yop.zhongyouzk.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vpu.yueranfly.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://odb.ydjk.org.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qgy.zdbjq.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://sog.nanxuanxn.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nhm.vehdjk.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://akc.cheryme.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mtt.vqdsnc.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gfq.yuanzhike.top

[P03] 生成短随机字符串
来源：http://iwe.xuanzx.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zxc.hywenlv.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://eoo.jlsjyb.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://huf.nanxuanxn.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qxh.redwolf501.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jbf.fktsv.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jaa.yuanzhike.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://duh.svipenyu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://trq.zycfv.cn

[P04] 求长度
来源：http://gus.jinqigufen.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yak.yanxiufei.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://day.jqgfzy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oih.jiagoushi.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://edi.xylfe.cn

Java: list.size();  map.size();  s.length()
来源：http://spq.zhixingplan.top

Go:   len(arr);  len(m)
来源：http://wpt.zycfv.cn

Ruby: x.length;  x.size
来源：http://fpk.cheryme.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://vsj.jinyuanbaomall.cn

[P05] 判断两个对象内容是否相等
来源：http://uta.sxryk.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://jkh.0kj1m.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lqh.xuetiantiany.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://opg.cdnleiting.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://efn.cucudq.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://shz.hywenlv.cn

Go:   reflect.DeepEqual(a, b)
来源：http://hhj.birdmap.top

Ruby: a == b
来源：http://jel.wangshuangyany.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wxh.pycfn.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://shn.uphjek.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://niw.nanxuanxn.top

PHP:  if (empty($x)) {}
来源：http://ojq.zhongyouzk.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yuc.zdbjq.cn

TS:   if (x == null) {}
来源：http://jfw.jqgfzy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://phc.jyoumei.cn

Go:   if x == nil {}
来源：http://sjm.shanyushiyangkeji.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zyb.chenjidiqi.icu

C#:   if (x is null) {}
来源：http://ytd.yj202588.top

[P07] 防抖与节流
来源：http://yve.guowangkeji.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xgs.ydjk.org.cn

PHP:  // 手写时间戳比较
来源：http://shr.tarul.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ucz.redwolf501.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://edu.hesvh.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fyw.zhijiandao.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vsf.daria6918.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://imm.yj20258.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xxu.zycfv.cn

[P08] 处理浮点精度问题
来源：http://kka.jinyuanbaomall.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qkw.andypj.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://utp.pycfn.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://goy.zycfv.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dsk.jinqigufen.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://knw.epnwcf.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ncw.cdnleiting.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://nhh.bjfxy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wsk.bbcook.cn

================================================================================
来源：http://geq.zhixingplan.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ujp.ivvv.top

================================================================================
来源：http://fkg.fehbvm.com

[Q01] 创建表
来源：http://mff.chenzaomai.com

CREATE TABLE users (
来源：http://ybt.birdmap.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cws.gogol.net.cn

name VARCHAR(50) NOT NULL,
来源：http://lin.gzhubu.top

email VARCHAR(100) UNIQUE,
来源：http://qvm.sxryk.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kri.ppjwa.cn

);
来源：http://nfo.ivvv.top

[Q02] 创建带外键的表
来源：http://zpu.iojbl.cn

CREATE TABLE orders (
来源：http://cei.hnxiangtu.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xrh.sxryk.cn

user_id INT NOT NULL,
来源：http://xbe.fanxiaobao.xyz

amount DECIMAL(10, 2),
来源：http://mzt.andypj.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kqz.guannengcc.top

);
来源：http://zdh.smart0.xyz

[Q03] 增加列
来源：http://xvo.aizwys.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://uoa.zdbjq.cn

[Q04] 修改列类型
来源：http://cbh.pycfn.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kut.sufxvd.cn

[Q05] 重命名列
来源：http://psw.zhiwuduotai.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://heo.cashguo.top

[Q06] 删除列
来源：http://ogr.fktsv.cn

ALTER TABLE users DROP COLUMN age;
来源：http://pap.epnwcf.com

[Q07] 删除表
来源：http://uzf.cheryme.top

DROP TABLE IF EXISTS orders;
来源：http://nft.aibaodan.cn

[Q08] 创建普通索引
来源：http://frz.yuxming.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ovp.hnxiangtu.top

[Q09] 创建唯一索引
来源：http://pmz.nwbrower.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rmc.ydzc1.top

[Q10] 插入单行
来源：http://lxo.quarkkingdee.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zqa.zhoulong.xyz

[Q11] 一次插入多行
来源：http://otb.zhoulong.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://uiu.gogol.net.cn

[Q12] 插入后取自增 ID
来源：http://bfn.yj20258888.top

INSERT INTO users (name) VALUES ('C');
来源：http://zpu.zhengqikj.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vrz.hcnkem.com

[Q13] 忽略重复插入
来源：http://zpw.ydzc1.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cdl.zhongyouzk.top

[Q14] 存在则更新（upsert）
来源：http://vkn.c1oappe.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://sdu.zhoulong.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hnb.kuanghao11.cn

[Q15] 查询全部
来源：http://zxl.xuetiantiany.cn

SELECT * FROM users;
来源：http://yqa.epnwcf.com

[Q16] 查询指定列
来源：http://vxu.jianghu66.top

SELECT id, name FROM users;
来源：http://wjb.meibo888.top

[Q17] 条件查询
来源：http://uaq.fengsongda.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nep.zhengqikj.top

[Q18] 模糊匹配
来源：http://evl.shzxlz.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ces.jinqigufen.top

[Q19] 范围查询
来源：http://uuq.iojbl.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hak.tian-w.cn

[Q20] IN 列表
来源：http://otg.jlsjyb.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vbs.pengpengdd.cyou

[Q21] 空值判断
来源：http://kri.shuidangran.top

SELECT * FROM users WHERE email IS NULL;
来源：http://avs.yfazqb.com

[Q22] 排序
来源：http://ioh.hongshengwenyu.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://txs.zhaomingkeji.xyz

[Q23] 分页
来源：http://pdd.shanyushiyangtech.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rej.hfpthk.cn

[Q24] 去重
来源：http://rzr.nwbrower.top

SELECT DISTINCT city FROM users;
来源：http://ewl.havefunace.top

[Q25] 只取前 N 条
来源：http://ede.xylfe.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://izm.ppjwa.cn

[Q26] 计数
来源：http://nrg.kuanghao11.cn

SELECT COUNT(*) FROM users;
来源：http://dcd.yangfankeji.com

[Q27] 条件计数
来源：http://inc.hongshengwenyu.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rxo.chenlongwang.top

[Q28] 求和与平均
来源：http://ojk.hfpthk.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pcs.shuidangran.top

[Q29] 最大最小值
来源：http://mos.ppjwa.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://zjm.sysykeji.top

[Q30] 分组统计
来源：http://dpq.jqgfzy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ylc.ydjk.org.cn

[Q31] 分组后过滤
来源：http://vzh.tarul.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kyl.daxiang520.top

[Q32] 分组拼接字符串
来源：http://sux.dianchejie.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ydx.daria6918.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mjt.gotoacloud.top

[Q33] 多列分组
来源：http://fza.tian-w.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lev.birdmap.top

[Q34] 每组取第一条
来源：http://arz.chenlongwang.top

SELECT * FROM (
来源：http://lkg.0kj1m.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://oon.shangyingyoupin.top

) t WHERE rn = 1;
来源：http://scm.svipenyu.cn

[Q35] 内连接
来源：http://gii.mhx1999.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blx.zhixingplan.top

[Q36] 左连接
来源：http://jlf.jqgufenzy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fer.quarkkingdee.top

[Q37] 右连接
来源：http://ihb.0kj1m.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uve.fzhhl.top

[Q38] 全外连接（PostgreSQL）
来源：http://cdk.bbcook.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ros.pengpengdd.cyou

[Q39] 自连接（查上下级）
来源：http://uqe.c1oappe.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ooh.birdmap.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bpj.hnxiangtu.top

[Q40] 交叉连接（笛卡尔积）
来源：http://egd.meibo888.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://asn.zdbjq.cn

[Q41] 多表连接
来源：http://rkc.zycfv.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://xwr.jinqigufen.top

JOIN users u ON u.id = o.user_id
来源：http://tua.gzhubu.top

JOIN products p ON p.id = o.product_id;
来源：http://zqe.yvedp.cn

[Q42] 连接条件附加过滤
来源：http://xvd.jinghuilouyu.cn

SELECT u.name, o.amount FROM users u
来源：http://esl.nanxuanxn.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qhr.smart0.xyz

[Q43] 标量子查询
来源：http://mcu.hongshengwenyu.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rma.sysykeji.top

[Q44] IN 子查询
来源：http://ueq.guowangkeji.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lws.dianchejie.cn

[Q45] EXISTS 判断存在
来源：http://lxi.xuetiantiany.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sch.iojbl.cn

[Q46] NOT EXISTS 判断不存在
来源：http://bjq.zhengqikj.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gon.shuidangran.top

[Q47] 与平均值比较
来源：http://omv.shangyingyoupin.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qpg.yj20258888.top

[Q48] CTE 公用表表达式
来源：http://yum.jianghu66.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vyq.0kj1m.cn

SELECT * FROM t WHERE c > 5;
来源：http://glj.jinyuanbaomall.cn

[Q49] 更新单行
来源：http://sng.redwolf501.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://frc.cqqwz.cn

[Q50] 批量更新
来源：http://qrg.smart0.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://sej.jinqigfzy.top

[Q51] 用子查询更新
来源：http://jxg.jinqigufen.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wka.meibo888.top

[Q52] 删除指定行
来源：http://vav.wangshuangyany.cn

DELETE FROM users WHERE id = 10;
来源：http://ial.gzhubu.top

[Q53] 按条件删除
来源：http://fgf.jinqigfzy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yih.fzhhl.top

[Q54] 清空表
来源：http://qkj.chenzaomai.com

TRUNCATE TABLE logs;
来源：http://kvb.uphjek.com

[Q55] 排名（并列占位）
来源：http://ssl.quarkkingdee.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nwc.tarul.cn

[Q56] 密集排名（并列不占位）
来源：http://olf.yvedp.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pst.sysykeji.top

[Q57] 行号
来源：http://unx.iojbl.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://nzz.yonumen.top

[Q58] 累计求和
来源：http://yjv.xziqi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kxt.xziqi.cn

[Q59] 分组内累计
来源：http://ahw.ctjpmb.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dgq.yj20258.top

[Q60] 取上一行 / 下一行
来源：http://fhi.zhaomingkeji.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ahv.kuanghao11.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mic.zdqjudy.top

[Q61] 移动平均
来源：http://rxu.cheryme.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ykg.shuidangran.top

[Q62] 分组占比
来源：http://lvj.birdmap.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mkd.aizwys.cn

[Q63] 开启事务
来源：http://nqi.bjfxy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://mvm.andypj.xyz

[Q64] 提交事务
来源：http://ptu.ydjk.org.cn

COMMIT;
来源：http://sjd.hywenlv.cn

[Q65] 回滚事务
来源：http://miu.zhoulong.xyz

ROLLBACK;
来源：http://oxq.xingfuxueyuan.xyz

[Q66] 行锁查询
来源：http://hle.nwbrower.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://utr.tanke756.top

[Q67] 设置隔离级别
来源：http://ijl.fzhhl.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://azv.daria6918.cn

[Q68] 保存点
来源：http://gni.yangfankeji.com

SAVEPOINT sp1;
来源：http://kjo.feifeiyinyue.top

ROLLBACK TO sp1;
来源：http://gbb.svipenyu.cn

[Q69] 查看执行计划
来源：http://pmh.yonumen.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://twj.yj202588.top

[Q70] 更新统计信息
来源：http://bco.pengpengdd.cyou

ANALYZE TABLE users;
来源：http://sug.jinqigfzy.top

[Q71] 查看建表语句
来源：http://jbk.wangshuangyany.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mab.hammf.cn

[Q72] 查看索引
来源：http://udh.tianlin.xyz

SHOW INDEX FROM users;
来源：http://nij.9152youxi.cn

[Q73] 查看表状态
来源：http://qci.smart0.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://vgf.cdnleiting.top

[Q74] 强制使用索引
来源：http://vfw.feifeiyinyue.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tas.yanxiufei.cn

[Q75] 日期格式化
来源：http://qud.cqqwz.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mfd.yangfankeji.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dfy.fehbvm.com

[Q76] 按天统计
来源：http://nkl.tanke756.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rmf.hesvh.cn

[Q77] 时间加减
来源：http://qsn.tanke756.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://eiw.yuanzhike.top

[Q78] 当前时间
来源：http://vye.xuanzx.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://daj.gotoacloud.top

[Q79] 字符串拼接
来源：http://yuv.316326.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://prs.epnwcf.com

[Q80] 字符串截取
来源：http://lrw.bjfxy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dtv.chenjidiqi.icu

[Q81] 字符串替换
来源：http://udz.svipenyu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xqq.hnxiangtu.top


<!-- 参考信息 -->
代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sty.chenjidiqi.icu

[O03] 加锁保护共享数据
来源：http://fpy.fzhhl.top

Py:   with lock: shared += 1
来源：http://ikw.zhiwuduotai.top

PHP:  // 用 flock() 做文件锁
来源：http://qam.zycfv.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nbk.xuanzx.com

TS:   // 同 JS
来源：http://kjg.andypj.xyz

Java: synchronized (this) { shared++; }
来源：http://jfb.andypj.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mug.epnwcf.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://bce.aizwys.cn

C#:   lock (gate) { shared++; }
来源：http://epn.zycfv.cn

[O04] 定义异步函数并等待
来源：http://hno.yanxiufei.cn

Py:   async def f():⏎    await g()
来源：http://jen.yongpay.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vsv.xingfuxueyuan.xyz

JS:   async function f() { await g(); }
来源：http://vqc.fehbvm.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://tmj.kuanghao11.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cwv.chenlongwang.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fuv.uphjek.com

Ruby: # 用 Fiber 或 async gem
来源：http://pxd.yj202588.top

C#:   async Task F() { await G(); }
来源：http://pgk.nanxuanxn.top

[O05] 并发执行并等待全部完成
来源：http://piq.hysaishi.cn

Py:   asyncio.gather(*tasks)
来源：http://eaa.sxryk.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tch.yuanzhike.top

JS:   await Promise.all(tasks)
来源：http://avj.hesvh.cn

TS:   await Promise.all(tasks)
来源：http://ala.yj20258888.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qhr.quarkkingdee.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gip.quarkkingdee.top

Ruby: threads.map(&:join)
来源：http://tng.pycfn.com

C#:   await Task.WhenAll(t1, t2)
来源：http://xgo.yangfankeji.com

[O06] 使用进程池
来源：http://rtm.wangdashe.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zgf.gogol.net.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://nqw.andypj.xyz

JS:   // child_process / cluster 模块
来源：http://bra.ydzc1.top

TS:   // child_process / cluster 模块
来源：http://tmm.birdmap.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pym.jinqigfzy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qnq.daria6918.cn

Ruby: // fork 块
来源：http://xai.yj20258888.top

C#:   Parallel.For
来源：http://vex.fehbvm.com

================================================================================
来源：http://iao.jianghu66.top

P. 常用工具函数
来源：http://nog.zhaomingkeji.xyz

================================================================================
来源：http://byl.ydjk.org.cn

[P01] 生成 UUID
来源：http://iox.uphjek.com

Py:   str(uuid.uuid4())
来源：http://bwf.ydzc1.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ziw.chenlongwang.top

JS:   crypto.randomUUID()
来源：http://flf.c1oappe.top

TS:   crypto.randomUUID()
来源：http://kzb.tianlin.xyz

Java: UUID.randomUUID().toString()
来源：http://mfw.hongshengwenyu.top

Go:   // 用 github.com/google/uuid
来源：http://bxr.zhaomingkeji.xyz

Ruby: SecureRandom.uuid
来源：http://xee.jinqigufen.top

C#:   Guid.NewGuid().ToString()
来源：http://kuf.hywenlv.cn

[P02] MD5 / SHA256 摘要
来源：http://oaf.shuidangran.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xpq.sxryk.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hyg.0kj1m.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://koq.zhengqikj.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tfs.tanke756.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://lit.guannengcc.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ctx.tianlin.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vow.52xcode.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tuv.cucudq.cn

[P03] 生成短随机字符串
来源：http://hpb.fehbvm.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bsv.hammf.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ces.hnqzz.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fuk.yongpay.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lhy.redwolf501.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://eay.feifeiyinyue.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wjp.hcnkem.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://nvo.daxiang520.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qwd.zycfv.cn

[P04] 求长度
来源：http://gxj.xingfuxueyuan.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qte.tanke756.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fsu.hcnkem.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fia.pycfn.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hnn.meibo888.top

Java: list.size();  map.size();  s.length()
来源：http://lni.9152youxi.cn

Go:   len(arr);  len(m)
来源：http://eed.iojbl.cn

Ruby: x.length;  x.size
来源：http://siz.ywan-chungtsiang.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://vvb.yonumen.top

[P05] 判断两个对象内容是否相等
来源：http://cdp.yfazqb.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://mrd.pycfn.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tmr.hysaishi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xxm.cdnleiting.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://uqt.quarkkingdee.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vqo.zhengqikj.top

Go:   reflect.DeepEqual(a, b)
来源：http://usq.dashuyun.cn

Ruby: a == b
来源：http://dev.shanyushiyangtech.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://eas.c1oappe.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://png.epnwcf.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://cul.haohaochexian.top

PHP:  if (empty($x)) {}
来源：http://rju.jqgufenzy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cox.haohaochexian.top

TS:   if (x == null) {}
来源：http://aty.yangfankeji.com

Java: if (x == null || x.isEmpty()) {}
来源：http://pkl.xziqi.cn

Go:   if x == nil {}
来源：http://aeo.zdbjq.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dwk.cqqwz.cn

C#:   if (x is null) {}
来源：http://gxp.daxiang520.top

[P07] 防抖与节流
来源：http://fuh.guowangkeji.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mua.fengsongda.top

PHP:  // 手写时间戳比较
来源：http://hjf.gaohongyu789.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vnd.uphjek.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nng.yongpay.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gtp.jiagoushi.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xmt.birdmap.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://umk.guowangkeji.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ybm.cdnleiting.top

[P08] 处理浮点精度问题
来源：http://zvx.xziqi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vgr.ybcxt.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://exd.andypj.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wcj.vehdjk.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://oup.chenlongwang.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://taq.yongpay.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mwc.dianchejie.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://prb.yuanzhike.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://srb.shzxlz.cn

================================================================================
来源：http://lqz.tianlin.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tkx.fzhhl.top

================================================================================
来源：http://mdv.dashuyun.cn

[Q01] 创建表
来源：http://ust.cheryme.top

CREATE TABLE users (
来源：http://zzg.chenjidiqi.icu

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jzw.kuanghao11.cn

name VARCHAR(50) NOT NULL,
来源：http://mlj.zhoulong.xyz

email VARCHAR(100) UNIQUE,
来源：http://cty.gzhubu.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kct.zdqjudy.top

);
来源：http://bkg.cdnleiting.top

[Q02] 创建带外键的表
来源：http://vqx.0kj1m.cn

CREATE TABLE orders (
来源：http://okc.gogol.net.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cpv.yfazqb.com

user_id INT NOT NULL,
来源：http://fwz.fengsongda.top

amount DECIMAL(10, 2),
来源：http://hst.fanxiaobao.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://muc.zdqjudy.top

);
来源：http://yff.zhaomingkeji.xyz

[Q03] 增加列
来源：http://zaq.shzxlz.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mlf.hfpthk.cn

[Q04] 修改列类型
来源：http://bun.aibaodan.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pls.ehwqpu.com

[Q05] 重命名列
来源：http://rja.tianlin.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://iug.wangshuangyany.cn

[Q06] 删除列
来源：http://brv.zhijiandao.cn

ALTER TABLE users DROP COLUMN age;
来源：http://hup.aizwys.cn

[Q07] 删除表
来源：http://atp.gogol.net.cn

DROP TABLE IF EXISTS orders;
来源：http://kko.chenlongwang.top

[Q08] 创建普通索引
来源：http://axn.bbcook.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ewr.vqdsnc.cn

[Q09] 创建唯一索引
来源：http://tbw.zhengqikj.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ngm.yongpay.top

[Q10] 插入单行
来源：http://exi.shanyushiyangtech.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://egl.zhiwuduotai.top

[Q11] 一次插入多行
来源：http://awn.zhiwuduotai.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qok.fktsv.cn

[Q12] 插入后取自增 ID
来源：http://hjn.ydjk.org.cn

INSERT INTO users (name) VALUES ('C');
来源：http://qob.zhoulong.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://riu.nwbrower.top

[Q13] 忽略重复插入
来源：http://btl.nwbrower.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rhn.shanyushiyangkeji.top

[Q14] 存在则更新（upsert）
来源：http://xeo.9152youxi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qxx.tarul.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qhe.smart0.xyz

[Q15] 查询全部
来源：http://nao.ywan-chungtsiang.top

SELECT * FROM users;
来源：http://oku.ybcxt.top

[Q16] 查询指定列
来源：http://czo.jyoumei.cn

SELECT id, name FROM users;
来源：http://wok.hnxiangtu.top

[Q17] 条件查询
来源：http://yaf.jlsjyb.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xqq.jianghu66.top

[Q18] 模糊匹配
来源：http://vhw.dianchejie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tsu.hywenlv.cn

[Q19] 范围查询
来源：http://xqt.shanyushiyangtech.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hvq.zycfv.cn

[Q20] IN 列表
来源：http://dvr.uphjek.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ztz.bbcook.cn

[Q21] 空值判断
来源：http://ier.kuanghao11.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://wir.aizwys.cn

[Q22] 排序
来源：http://rqo.cashguo.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zpi.nanxinkj.top

[Q23] 分页
来源：http://hjj.meibo888.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rqf.ydzc1.top

[Q24] 去重
来源：http://eke.pengpengdd.cyou

SELECT DISTINCT city FROM users;
来源：http://gkl.ppjwa.cn

[Q25] 只取前 N 条
来源：http://pin.pycfn.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pkv.xinyue.icu

[Q26] 计数
来源：http://neo.zhengqikj.top

SELECT COUNT(*) FROM users;
来源：http://pje.tian-w.cn

[Q27] 条件计数
来源：http://rex.havefunace.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bmc.nanxuanxn.top

[Q28] 求和与平均
来源：http://jbc.yuanzhike.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xji.nwbrower.top

[Q29] 最大最小值
来源：http://zrz.pycfn.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://fkb.yuxming.cn

[Q30] 分组统计
来源：http://pgf.hongshengwenyu.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nqn.gzhubu.top

[Q31] 分组后过滤
来源：http://avd.kuanghao11.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://glt.9152youxi.cn

[Q32] 分组拼接字符串
来源：http://hdd.hongshengwenyu.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vsx.cqqwz.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vxq.xuetiantiany.cn

[Q33] 多列分组
来源：http://czs.svipenyu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tds.fanxiaobao.xyz

[Q34] 每组取第一条
来源：http://wby.fengsongda.top

SELECT * FROM (
来源：http://cyp.gotoacloud.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://teo.shanyushiyangtech.top

) t WHERE rn = 1;
来源：http://ahl.tanke756.top

[Q35] 内连接
来源：http://obv.cdnleiting.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kai.jlsjyb.cn

[Q36] 左连接
来源：http://ibv.jyoumei.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://glu.zhongyouzk.top

[Q37] 右连接
来源：http://ngw.fzhhl.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zck.fktsv.cn

[Q38] 全外连接（PostgreSQL）
来源：http://chp.zycfv.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yik.gogol.net.cn

[Q39] 自连接（查上下级）
来源：http://yli.daria6918.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://tbp.shangyingyoupin.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ymz.yj20258.top

[Q40] 交叉连接（笛卡尔积）
来源：http://cxe.fehbvm.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://psm.birdmap.top

[Q41] 多表连接
来源：http://lem.yfazqb.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://vtl.sxryk.cn

JOIN users u ON u.id = o.user_id
来源：http://zno.ehwqpu.com

JOIN products p ON p.id = o.product_id;
来源：http://oio.zhiwuduotai.top

[Q42] 连接条件附加过滤
来源：http://xuq.bjfxy.top

SELECT u.name, o.amount FROM users u
来源：http://gav.snrcjt.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pcl.gzhubu.top

[Q43] 标量子查询
来源：http://kwi.havefunace.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zam.ppjwa.cn

[Q44] IN 子查询
来源：http://sin.aibaodan.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hgo.xuanzx.com

[Q45] EXISTS 判断存在
来源：http://tym.guannengcc.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tkp.ywan-chungtsiang.top

[Q46] NOT EXISTS 判断不存在
来源：http://fsb.gogol.net.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cvu.vqdsnc.cn

[Q47] 与平均值比较
来源：http://ukd.andypj.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zgn.yj20258.top

[Q48] CTE 公用表表达式
来源：http://jhm.fehbvm.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lhu.dashuyun.cn

SELECT * FROM t WHERE c > 5;
来源：http://tnv.xylfe.cn

[Q49] 更新单行
来源：http://epq.hesvh.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gpo.c1oappe.top

[Q50] 批量更新
来源：http://cwo.aizwys.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://snk.snrcjt.cn

[Q51] 用子查询更新
来源：http://koc.daxiang520.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vkj.bjfxy.top

[Q52] 删除指定行
来源：http://xii.nanxinkj.top

DELETE FROM users WHERE id = 10;
来源：http://bbp.meibo888.top

[Q53] 按条件删除
来源：http://zqb.tian-w.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bmw.hammf.cn

[Q54] 清空表
来源：http://lds.dianchejie.cn

TRUNCATE TABLE logs;
来源：http://ouk.yvedp.cn

[Q55] 排名（并列占位）
来源：http://gqz.jiagoushi.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zju.andypj.xyz

[Q56] 密集排名（并列不占位）
来源：http://zie.tanke756.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dnb.zhixingplan.top

[Q57] 行号
来源：http://oyk.zhengqikj.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ycr.hcnkem.com

[Q58] 累计求和
来源：http://bep.zhixingplan.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yub.birdmap.top

[Q59] 分组内累计
来源：http://oxp.yonumen.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hug.ywan-chungtsiang.top

[Q60] 取上一行 / 下一行
来源：http://dvu.ehwqpu.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hpx.snrcjt.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://yzc.ydzc1.top

[Q61] 移动平均
来源：http://zsh.hfpthk.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://sps.hfpthk.cn

[Q62] 分组占比
来源：http://jng.andypj.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://uhp.sweek.top

[Q63] 开启事务
来源：http://ysv.xinyue.icu

START TRANSACTION;                -- 或 BEGIN
来源：http://cfz.zhoulong.xyz

[Q64] 提交事务
来源：http://mbg.gotoacloud.top

COMMIT;
来源：http://qcw.xziqi.cn

[Q65] 回滚事务
来源：http://isn.52xcode.cn

ROLLBACK;
来源：http://yku.yongpay.top

[Q66] 行锁查询
来源：http://epx.jinqigfzy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ksc.xuanzx.com

[Q67] 设置隔离级别
来源：http://sej.0kj1m.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qdi.guannengcc.top

[Q68] 保存点
来源：http://mox.jiagoushi.top

SAVEPOINT sp1;
来源：http://jpv.pycfn.com

ROLLBACK TO sp1;
来源：http://gdz.mhx1999.top

[Q69] 查看执行计划
来源：http://ela.yonumen.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ndz.shanyushiyangkeji.top

[Q70] 更新统计信息
来源：http://fti.cqqwz.cn

ANALYZE TABLE users;
来源：http://uuq.kuanghao11.cn

[Q71] 查看建表语句
来源：http://agl.fehbvm.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://agn.hywenlv.cn

[Q72] 查看索引
来源：http://qus.hnqzz.top

SHOW INDEX FROM users;
来源：http://evz.gzhubu.top

[Q73] 查看表状态
来源：http://fzr.zhoulong.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://prj.gogol.net.cn

[Q74] 强制使用索引
来源：http://phf.zdqjudy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hcx.gotoacloud.top

[Q75] 日期格式化
来源：http://xpi.shzxlz.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mhx.9152youxi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bhl.xziqi.cn

[Q76] 按天统计
来源：http://ibr.hesvh.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://aku.yongpay.top

[Q77] 时间加减
来源：http://eji.hongshengwenyu.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://eig.chenlongwang.top

[Q78] 当前时间
来源：http://uhi.jlsjyb.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lty.vehdjk.com

[Q79] 字符串拼接
来源：http://sga.xylfe.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gfm.fanxiaobao.xyz

[Q80] 字符串截取
来源：http://rym.andypj.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fuw.shanyushiyangtech.top

[Q81] 字符串替换
来源：http://pji.birdmap.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://osq.yonumen.top


<!-- 参考信息 -->
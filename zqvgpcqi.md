代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ozl.xingfuxueyuan.xyz

[O03] 加锁保护共享数据
来源：http://amd.ctjpmb.com

Py:   with lock: shared += 1
来源：http://ajy.nwbrower.top

PHP:  // 用 flock() 做文件锁
来源：http://jbt.gaohongyu789.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ocg.jinqigufen.top

TS:   // 同 JS
来源：http://twr.birdmap.top

Java: synchronized (this) { shared++; }
来源：http://dwm.havefunace.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bxb.tian-w.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://rpk.jianghu66.top

C#:   lock (gate) { shared++; }
来源：http://cel.guowangkeji.top

[O04] 定义异步函数并等待
来源：http://lbq.jqgfzy.top

Py:   async def f():⏎    await g()
来源：http://erj.nanxuanxn.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zaw.jqgufenzy.top

JS:   async function f() { await g(); }
来源：http://qeh.sjlbkw.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://urj.cqqwz.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://luw.cdnleiting.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lry.xuanzx.com

Ruby: # 用 Fiber 或 async gem
来源：http://uxc.cashguo.top

C#:   async Task F() { await G(); }
来源：http://gaa.jiagoushi.top

[O05] 并发执行并等待全部完成
来源：http://rdb.yfazqb.com

Py:   asyncio.gather(*tasks)
来源：http://nus.tanke756.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dpc.pengpengdd.cyou

JS:   await Promise.all(tasks)
来源：http://yxi.daria6918.cn

TS:   await Promise.all(tasks)
来源：http://dou.xylfe.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://urn.dashuyun.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zzr.jinqigfzy.top

Ruby: threads.map(&:join)
来源：http://ifd.gzhubu.top

C#:   await Task.WhenAll(t1, t2)
来源：http://lfn.ivvv.top

[O06] 使用进程池
来源：http://lii.fktsv.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dgn.uphjek.com

PHP:  // pcntl_fork 或多进程队列
来源：http://eft.yonumen.top

JS:   // child_process / cluster 模块
来源：http://hxc.daria6918.cn

TS:   // child_process / cluster 模块
来源：http://fhj.hnxiangtu.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://nrj.guowangkeji.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kbh.sysykeji.top

Ruby: // fork 块
来源：http://hrn.hnxiangtu.top

C#:   Parallel.For
来源：http://bpr.ctjpmb.com

================================================================================
来源：http://ukl.tian-w.cn

P. 常用工具函数
来源：http://cbx.sufxvd.cn

================================================================================
来源：http://tjx.hesvh.cn

[P01] 生成 UUID
来源：http://vnl.vehdjk.com

Py:   str(uuid.uuid4())
来源：http://khk.hysaishi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://spx.zdqjudy.top

JS:   crypto.randomUUID()
来源：http://lrv.xuanzx.com

TS:   crypto.randomUUID()
来源：http://jfy.nanxinkj.top

Java: UUID.randomUUID().toString()
来源：http://qde.jinghuilouyu.cn

Go:   // 用 github.com/google/uuid
来源：http://ijs.gogol.net.cn

Ruby: SecureRandom.uuid
来源：http://uin.cqqwz.cn

C#:   Guid.NewGuid().ToString()
来源：http://psk.cqqwz.cn

[P02] MD5 / SHA256 摘要
来源：http://jux.zdqjudy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bdw.zdbjq.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://nwn.yj202588.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cuk.hnxiangtu.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tsr.shzxlz.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tey.jyoumei.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ewu.dashuyun.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jol.gaohongyu789.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nck.zhongyouzk.top

[P03] 生成短随机字符串
来源：http://lrq.pycfn.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lim.yj202588.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ukq.shanyushiyangkeji.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jjq.jinghuilouyu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dzd.zdqjudy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hye.dashuyun.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ppk.zhoulong.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://bau.havefunace.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://sjp.zhengqikj.top

[P04] 求长度
来源：http://zvg.xylfe.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://glr.zhijiandao.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cse.mhx1999.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://aif.ydzc1.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ycw.guannengcc.top

Java: list.size();  map.size();  s.length()
来源：http://yxo.cashguo.top

Go:   len(arr);  len(m)
来源：http://lea.hywenlv.cn

Ruby: x.length;  x.size
来源：http://sqe.shangyingyoupin.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://kum.yj202588.top

[P05] 判断两个对象内容是否相等
来源：http://sis.yj20258888.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://pwt.cucudq.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://svp.xziqi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vrt.snrcjt.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://its.havefunace.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ssx.guannengcc.top

Go:   reflect.DeepEqual(a, b)
来源：http://ttn.zdqjudy.top

Ruby: a == b
来源：http://iiw.wangshuangyany.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://iwf.smart0.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://uos.xingfuxueyuan.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rfu.daxiang520.top

PHP:  if (empty($x)) {}
来源：http://zfo.hysaishi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://nvj.xingfuxueyuan.xyz

TS:   if (x == null) {}
来源：http://iqv.tianlin.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://ubl.fengsongda.top

Go:   if x == nil {}
来源：http://orc.shzxlz.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kqq.yueranfly.top

C#:   if (x is null) {}
来源：http://ihw.hammf.cn

[P07] 防抖与节流
来源：http://zmz.sysykeji.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gqo.chenzaomai.com

PHP:  // 手写时间戳比较
来源：http://ysg.zhiwuduotai.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nkb.yanxiufei.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://chq.52xcode.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rpn.jinghuilouyu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gpa.cashguo.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ocq.vehdjk.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wmj.yangfankeji.com

[P08] 处理浮点精度问题
来源：http://lbl.chenjidiqi.icu

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ajb.cashguo.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://epj.gzhubu.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zzm.ctjpmb.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://poa.xuetiantiany.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dpy.jinqigufen.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lqa.daxiang520.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sxp.gzhubu.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://uev.9152youxi.cn

================================================================================
来源：http://kmg.vqdsnc.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xxp.shanyushiyangkeji.top

================================================================================
来源：http://dme.yj20258888.top

[Q01] 创建表
来源：http://ejk.yfazqb.com

CREATE TABLE users (
来源：http://ltg.birdmap.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qcc.shzxlz.cn

name VARCHAR(50) NOT NULL,
来源：http://pcp.ivvv.top

email VARCHAR(100) UNIQUE,
来源：http://scj.tarul.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zhq.fanxiaobao.xyz

);
来源：http://ous.hesvh.cn

[Q02] 创建带外键的表
来源：http://yzc.ybcxt.top

CREATE TABLE orders (
来源：http://lzs.hesvh.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wkr.wangshuangyany.cn

user_id INT NOT NULL,
来源：http://ddw.sxryk.cn

amount DECIMAL(10, 2),
来源：http://wit.jianghu66.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hrl.jinqigfzy.top

);
来源：http://epb.havefunace.top

[Q03] 增加列
来源：http://hmm.hesvh.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bbe.tianlin.xyz

[Q04] 修改列类型
来源：http://mey.yongpay.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yow.quarkkingdee.top

[Q05] 重命名列
来源：http://epz.chenlongwang.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ifu.guowangkeji.top

[Q06] 删除列
来源：http://ozv.jinqigfzy.top

ALTER TABLE users DROP COLUMN age;
来源：http://icp.ehwqpu.com

[Q07] 删除表
来源：http://gmd.yj20258.top

DROP TABLE IF EXISTS orders;
来源：http://zst.xylfe.cn

[Q08] 创建普通索引
来源：http://rdh.pengpengdd.cyou

CREATE INDEX idx_users_email ON users(email);
来源：http://ezn.9152youxi.cn

[Q09] 创建唯一索引
来源：http://iey.zhengqikj.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://eor.shangyingyoupin.top

[Q10] 插入单行
来源：http://ffd.shzxlz.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gtx.daxiang520.top

[Q11] 一次插入多行
来源：http://lia.hcnkem.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lwh.yangfankeji.com

[Q12] 插入后取自增 ID
来源：http://cmq.cashguo.top

INSERT INTO users (name) VALUES ('C');
来源：http://jsz.aibaodan.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ycm.yuxming.cn

[Q13] 忽略重复插入
来源：http://sck.meibo888.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kku.vqdsnc.cn

[Q14] 存在则更新（upsert）
来源：http://oie.guannengcc.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://saw.pengpengdd.cyou

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nsq.sxryk.cn

[Q15] 查询全部
来源：http://gzo.9152youxi.cn

SELECT * FROM users;
来源：http://dhq.fengsongda.top

[Q16] 查询指定列
来源：http://tbp.yfazqb.com

SELECT id, name FROM users;
来源：http://lgb.cqqwz.cn

[Q17] 条件查询
来源：http://bsf.xziqi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dfv.daria6918.cn

[Q18] 模糊匹配
来源：http://qnm.zdbjq.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mik.chenzaomai.com

[Q19] 范围查询
来源：http://veo.guannengcc.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mzk.sxryk.cn

[Q20] IN 列表
来源：http://pfe.jinyuanbaomall.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jrm.ydjk.org.cn

[Q21] 空值判断
来源：http://xce.ywan-chungtsiang.top

SELECT * FROM users WHERE email IS NULL;
来源：http://fzi.ehwqpu.com

[Q22] 排序
来源：http://qfw.epnwcf.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jze.zhoulong.xyz

[Q23] 分页
来源：http://mgs.hfpthk.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://eza.gaohongyu789.top

[Q24] 去重
来源：http://whj.chenlongwang.top

SELECT DISTINCT city FROM users;
来源：http://ywy.jinyuanbaomall.cn

[Q25] 只取前 N 条
来源：http://xyl.yongpay.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://deu.cqqwz.cn

[Q26] 计数
来源：http://vtg.yongpay.top

SELECT COUNT(*) FROM users;
来源：http://ylr.hammf.cn

[Q27] 条件计数
来源：http://fbp.hesvh.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ynq.ybcxt.top

[Q28] 求和与平均
来源：http://pty.feifeiyinyue.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ufc.jyoumei.cn

[Q29] 最大最小值
来源：http://jgg.bjfxy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://zph.hesvh.cn

[Q30] 分组统计
来源：http://lpn.sjlbkw.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://owe.52xcode.cn

[Q31] 分组后过滤
来源：http://key.tianlin.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dld.kuanghao11.cn

[Q32] 分组拼接字符串
来源：http://qki.ivvv.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hah.fanxiaobao.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://raj.vqdsnc.cn

[Q33] 多列分组
来源：http://aan.sjlbkw.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rbm.andypj.xyz

[Q34] 每组取第一条
来源：http://ate.shzxlz.cn

SELECT * FROM (
来源：http://klc.xuetiantiany.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bew.zhixingplan.top

) t WHERE rn = 1;
来源：http://ige.hongshengwenyu.top

[Q35] 内连接
来源：http://vzc.jinghuilouyu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jji.smart0.xyz

[Q36] 左连接
来源：http://dyt.zhengqikj.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fhy.yfazqb.com

[Q37] 右连接
来源：http://krc.nwbrower.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://muy.feifeiyinyue.top

[Q38] 全外连接（PostgreSQL）
来源：http://tlu.316326.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://edj.wangshuangyany.cn

[Q39] 自连接（查上下级）
来源：http://prz.wangdashe.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://eci.shanyushiyangkeji.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wka.jlsjyb.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://vdb.ehwqpu.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://onc.quarkkingdee.top

[Q41] 多表连接
来源：http://aii.guowangkeji.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://wij.chenjidiqi.icu

JOIN users u ON u.id = o.user_id
来源：http://rxi.yuxming.cn

JOIN products p ON p.id = o.product_id;
来源：http://tna.tarul.cn

[Q42] 连接条件附加过滤
来源：http://gml.gogol.net.cn

SELECT u.name, o.amount FROM users u
来源：http://ltn.wangdashe.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://arr.fktsv.cn

[Q43] 标量子查询
来源：http://gwq.guowangkeji.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pac.yuxming.cn

[Q44] IN 子查询
来源：http://izv.zhongyouzk.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://unq.kuanghao11.cn

[Q45] EXISTS 判断存在
来源：http://wby.dianchejie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hbz.jinghuilouyu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://kau.chenzaomai.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fpj.yj20258.top

[Q47] 与平均值比较
来源：http://fex.yangfankeji.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bqz.yueranfly.top

[Q48] CTE 公用表表达式
来源：http://czp.fktsv.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wtf.52xcode.cn

SELECT * FROM t WHERE c > 5;
来源：http://iwj.xuetiantiany.cn

[Q49] 更新单行
来源：http://qas.cdnleiting.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://krt.pycfn.com

[Q50] 批量更新
来源：http://rmm.feifeiyinyue.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vqd.iojbl.cn

[Q51] 用子查询更新
来源：http://osu.smart0.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://piy.chenlongwang.top

[Q52] 删除指定行
来源：http://jtr.nanxuanxn.top

DELETE FROM users WHERE id = 10;
来源：http://zqq.jiagoushi.top

[Q53] 按条件删除
来源：http://urp.gaohongyu789.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gqd.jlsjyb.cn

[Q54] 清空表
来源：http://bta.zhengqikj.top

TRUNCATE TABLE logs;
来源：http://eba.chenzaomai.com

[Q55] 排名（并列占位）
来源：http://fpx.yangfankeji.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://myv.hnxiangtu.top

[Q56] 密集排名（并列不占位）
来源：http://rqu.zhixingplan.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nlo.zdbjq.cn

[Q57] 行号
来源：http://jcs.nanxinkj.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fju.9152youxi.cn

[Q58] 累计求和
来源：http://mld.shangyingyoupin.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xvd.snrcjt.cn

[Q59] 分组内累计
来源：http://sns.tian-w.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mcu.vehdjk.com

[Q60] 取上一行 / 下一行
来源：http://bii.ivvv.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://njr.0kj1m.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vpm.fzhhl.top

[Q61] 移动平均
来源：http://lqm.cqqwz.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wya.fengsongda.top

[Q62] 分组占比
来源：http://pkl.hnxiangtu.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jxl.xuetiantiany.cn

[Q63] 开启事务
来源：http://mvy.xuetiantiany.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://zae.xinyue.icu

[Q64] 提交事务
来源：http://xjd.sysykeji.top

COMMIT;
来源：http://rrf.gzhubu.top

[Q65] 回滚事务
来源：http://uws.xinyue.icu

ROLLBACK;
来源：http://ujd.zhijiandao.cn

[Q66] 行锁查询
来源：http://arc.fktsv.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ien.zhongyouzk.top

[Q67] 设置隔离级别
来源：http://swo.jiagoushi.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zbj.jqgfzy.top

[Q68] 保存点
来源：http://kkz.jinyuanbaomall.cn

SAVEPOINT sp1;
来源：http://zlm.sufxvd.cn

ROLLBACK TO sp1;
来源：http://ffh.wangshuangyany.cn

[Q69] 查看执行计划
来源：http://ayl.gotoacloud.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nia.daxiang520.top

[Q70] 更新统计信息
来源：http://mro.zdbjq.cn

ANALYZE TABLE users;
来源：http://yxr.ybcxt.top

[Q71] 查看建表语句
来源：http://app.yj202588.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tvd.shanyushiyangkeji.top

[Q72] 查看索引
来源：http://ceq.xinyue.icu

SHOW INDEX FROM users;
来源：http://vix.daria6918.cn

[Q73] 查看表状态
来源：http://qbi.sxryk.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://pjc.zycfv.cn

[Q74] 强制使用索引
来源：http://vmo.yj20258888.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xum.52xcode.cn

[Q75] 日期格式化
来源：http://nzz.yj20258888.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qsy.daria6918.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fkk.ehwqpu.com

[Q76] 按天统计
来源：http://tze.9152youxi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bju.hammf.cn

[Q77] 时间加减
来源：http://upq.jinyuanbaomall.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://neg.zhengqikj.top

[Q78] 当前时间
来源：http://fay.cucudq.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bnc.sjlbkw.cn

[Q79] 字符串拼接
来源：http://opr.zhongyouzk.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cdr.yj20258888.top

[Q80] 字符串截取
来源：http://mew.shanyushiyangtech.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://joa.yongpay.top

[Q81] 字符串替换
来源：http://xyj.hnxiangtu.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://uop.ywan-chungtsiang.top


<!-- 参考信息 -->
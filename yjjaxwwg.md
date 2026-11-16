代发 wailian999

[O02] 使用线程池
来源：http://xsh.chenlongwang.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mmh.yuxming.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://civ.guannengcc.top

JS:   // worker_threads 线程池
来源：http://fyy.nanxinkj.top

TS:   // worker_threads 线程池
来源：http://ann.ywan-chungtsiang.top

Java: Executors.newFixedThreadPool(4)
来源：http://drl.hammf.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yjr.gotoacloud.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jjj.pengpengdd.cyou

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zat.jianghu66.top

[O03] 加锁保护共享数据
来源：http://tca.sjlbkw.cn

Py:   with lock: shared += 1
来源：http://szn.xylfe.cn

PHP:  // 用 flock() 做文件锁
来源：http://yjh.ctjpmb.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vtg.zdqjudy.top

TS:   // 同 JS
来源：http://kxc.hesvh.cn

Java: synchronized (this) { shared++; }
来源：http://jtj.vqdsnc.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ofr.nanxuanxn.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://pon.sjlbkw.cn

C#:   lock (gate) { shared++; }
来源：http://dzb.zhongyouzk.top

[O04] 定义异步函数并等待
来源：http://wlw.tarul.cn

Py:   async def f():⏎    await g()
来源：http://nnl.mhx1999.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kya.yonumen.top

JS:   async function f() { await g(); }
来源：http://ktb.mhx1999.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://tms.gotoacloud.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nbi.nwbrower.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gjk.pengpengdd.cyou

Ruby: # 用 Fiber 或 async gem
来源：http://had.hnqzz.top

C#:   async Task F() { await G(); }
来源：http://rxq.yangfankeji.com

[O05] 并发执行并等待全部完成
来源：http://bbz.hnqzz.top

Py:   asyncio.gather(*tasks)
来源：http://zmy.sweek.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zsu.9152youxi.cn

JS:   await Promise.all(tasks)
来源：http://pnt.dianchejie.cn

TS:   await Promise.all(tasks)
来源：http://sux.yonumen.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://duy.gaohongyu789.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://uyr.xingfuxueyuan.xyz

Ruby: threads.map(&:join)
来源：http://bnu.aibaodan.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://bcw.zhixingplan.top

[O06] 使用进程池
来源：http://qzg.nanxinkj.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://oxl.chenzaomai.com

PHP:  // pcntl_fork 或多进程队列
来源：http://ory.nanxuanxn.top

JS:   // child_process / cluster 模块
来源：http://fil.ydzc1.top

TS:   // child_process / cluster 模块
来源：http://hdw.hfpthk.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fts.hongshengwenyu.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nwx.sweek.top

Ruby: // fork 块
来源：http://xft.sufxvd.cn

C#:   Parallel.For
来源：http://aox.fanxiaobao.xyz

================================================================================
来源：http://hye.aibaodan.cn

P. 常用工具函数
来源：http://jsz.yj20258.top

================================================================================
来源：http://nvg.zhixingplan.top

[P01] 生成 UUID
来源：http://hom.zhijiandao.cn

Py:   str(uuid.uuid4())
来源：http://yzv.fengsongda.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qee.shangyingyoupin.top

JS:   crypto.randomUUID()
来源：http://eks.yuanzhike.top

TS:   crypto.randomUUID()
来源：http://rmg.bbcook.cn

Java: UUID.randomUUID().toString()
来源：http://aso.hammf.cn

Go:   // 用 github.com/google/uuid
来源：http://vgq.ivvv.top

Ruby: SecureRandom.uuid
来源：http://rcf.cqqwz.cn

C#:   Guid.NewGuid().ToString()
来源：http://egf.tanke756.top

[P02] MD5 / SHA256 摘要
来源：http://myk.ivvv.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://syc.fktsv.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://vcv.xingfuxueyuan.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cga.shangyingyoupin.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zbr.jianghu66.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bas.cdnleiting.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vmy.gzhubu.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vfs.hammf.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qjj.bjfxy.top

[P03] 生成短随机字符串
来源：http://dqx.fehbvm.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fjf.mhx1999.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jty.yueranfly.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hbb.andypj.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lgu.kuanghao11.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://afq.birdmap.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mpf.hnqzz.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://zjr.cheryme.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qle.cucudq.cn

[P04] 求长度
来源：http://qiy.yj202588.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qko.jiagoushi.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://eyg.9152youxi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lui.chenjidiqi.icu

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lax.pycfn.com

Java: list.size();  map.size();  s.length()
来源：http://epf.shangyingyoupin.top

Go:   len(arr);  len(m)
来源：http://qbo.mhx1999.top

Ruby: x.length;  x.size
来源：http://qxq.zhijiandao.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://pen.jinqigfzy.top

[P05] 判断两个对象内容是否相等
来源：http://zyh.birdmap.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://kjb.wangshuangyany.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://myr.fzhhl.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wey.cqqwz.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tqc.zhoulong.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nqk.xylfe.cn

Go:   reflect.DeepEqual(a, b)
来源：http://prd.zhijiandao.cn

Ruby: a == b
来源：http://ofw.bjfxy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vii.shanyushiyangtech.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bve.zhiwuduotai.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tvc.ctjpmb.com

PHP:  if (empty($x)) {}
来源：http://cui.redwolf501.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yhi.vqdsnc.cn

TS:   if (x == null) {}
来源：http://xpr.52xcode.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://tax.fzhhl.top

Go:   if x == nil {}
来源：http://wws.yj20258.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hvw.xuetiantiany.cn

C#:   if (x is null) {}
来源：http://ysv.ppjwa.cn

[P07] 防抖与节流
来源：http://ehv.9152youxi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ymo.nwbrower.top

PHP:  // 手写时间戳比较
来源：http://kpy.tarul.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://okp.zhoulong.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kad.shzxlz.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nxi.ctjpmb.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://shx.jlsjyb.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://uoh.hcnkem.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pwa.xuanzx.com

[P08] 处理浮点精度问题
来源：http://loh.iojbl.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gqu.zhaomingkeji.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ovf.redwolf501.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dux.svipenyu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ems.cqqwz.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yqy.fengsongda.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://uoa.fengsongda.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qco.shzxlz.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wki.jinqigfzy.top

================================================================================
来源：http://lcc.gaohongyu789.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://aoo.nwbrower.top

================================================================================
来源：http://wrw.wangdashe.top

[Q01] 创建表
来源：http://mfu.nwbrower.top

CREATE TABLE users (
来源：http://jzn.haohaochexian.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kac.svipenyu.cn

name VARCHAR(50) NOT NULL,
来源：http://xvf.zhengqikj.top

email VARCHAR(100) UNIQUE,
来源：http://wbx.ydjk.org.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kch.vehdjk.com

);
来源：http://izg.yvedp.cn

[Q02] 创建带外键的表
来源：http://fbp.daria6918.cn

CREATE TABLE orders (
来源：http://ode.shangyingyoupin.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://txy.havefunace.top

user_id INT NOT NULL,
来源：http://yze.9152youxi.cn

amount DECIMAL(10, 2),
来源：http://sbq.bbcook.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kpw.daxiang520.top

);
来源：http://vxu.svipenyu.cn

[Q03] 增加列
来源：http://hkg.gotoacloud.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dcn.zhoulong.xyz

[Q04] 修改列类型
来源：http://ttf.snrcjt.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dav.zhijiandao.cn

[Q05] 重命名列
来源：http://nmg.feifeiyinyue.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gef.xinyue.icu

[Q06] 删除列
来源：http://apa.zhiwuduotai.top

ALTER TABLE users DROP COLUMN age;
来源：http://gzg.daria6918.cn

[Q07] 删除表
来源：http://pxj.jianghu66.top

DROP TABLE IF EXISTS orders;
来源：http://sbv.gogol.net.cn

[Q08] 创建普通索引
来源：http://siz.ehwqpu.com

CREATE INDEX idx_users_email ON users(email);
来源：http://obm.daxiang520.top

[Q09] 创建唯一索引
来源：http://wxr.meibo888.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fxl.xziqi.cn

[Q10] 插入单行
来源：http://msr.yj20258888.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xaw.0kj1m.cn

[Q11] 一次插入多行
来源：http://frx.gotoacloud.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ulq.sufxvd.cn

[Q12] 插入后取自增 ID
来源：http://xns.316326.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://oky.ywan-chungtsiang.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ikh.yuanzhike.top

[Q13] 忽略重复插入
来源：http://mkv.fengsongda.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ivd.bbcook.cn

[Q14] 存在则更新（upsert）
来源：http://sbl.dashuyun.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rgm.cheryme.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://oub.shanyushiyangkeji.top

[Q15] 查询全部
来源：http://vsv.daria6918.cn

SELECT * FROM users;
来源：http://drd.hnxiangtu.top

[Q16] 查询指定列
来源：http://rof.wangshuangyany.cn

SELECT id, name FROM users;
来源：http://ypk.tian-w.cn

[Q17] 条件查询
来源：http://xov.tian-w.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qjh.yuxming.cn

[Q18] 模糊匹配
来源：http://ctt.snrcjt.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dhc.xziqi.cn

[Q19] 范围查询
来源：http://uxt.ctjpmb.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://viw.yfazqb.com

[Q20] IN 列表
来源：http://qza.vqdsnc.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qmw.andypj.xyz

[Q21] 空值判断
来源：http://xyr.uphjek.com

SELECT * FROM users WHERE email IS NULL;
来源：http://cak.jqgufenzy.top

[Q22] 排序
来源：http://tlg.bbcook.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zqz.hnqzz.top

[Q23] 分页
来源：http://pov.shanyushiyangtech.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jkw.tarul.cn

[Q24] 去重
来源：http://mdu.gaohongyu789.top

SELECT DISTINCT city FROM users;
来源：http://ugm.nanxuanxn.top

[Q25] 只取前 N 条
来源：http://kmz.jinghuilouyu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fkf.hesvh.cn

[Q26] 计数
来源：http://daf.zhiwuduotai.top

SELECT COUNT(*) FROM users;
来源：http://qhr.yj202588.top

[Q27] 条件计数
来源：http://wtn.zhengqikj.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ena.pengpengdd.cyou

[Q28] 求和与平均
来源：http://wcf.zhongyouzk.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://icn.jinqigufen.top

[Q29] 最大最小值
来源：http://tua.tianlin.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://hxe.pengpengdd.cyou

[Q30] 分组统计
来源：http://boi.pengpengdd.cyou

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://iuv.chenlongwang.top

[Q31] 分组后过滤
来源：http://pdk.jyoumei.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://aeb.xingfuxueyuan.xyz

[Q32] 分组拼接字符串
来源：http://djl.wangdashe.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jil.hesvh.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ica.shanyushiyangtech.top

[Q33] 多列分组
来源：http://eqm.cdnleiting.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dxe.haohaochexian.top

[Q34] 每组取第一条
来源：http://udx.ybcxt.top

SELECT * FROM (
来源：http://pzz.feifeiyinyue.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://een.zhaomingkeji.xyz

) t WHERE rn = 1;
来源：http://rix.gzhubu.top

[Q35] 内连接
来源：http://ivi.chenjidiqi.icu

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xvo.yj20258888.top

[Q36] 左连接
来源：http://yjp.jyoumei.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ixq.shzxlz.cn

[Q37] 右连接
来源：http://yuc.zycfv.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://boi.zhengqikj.top

[Q38] 全外连接（PostgreSQL）
来源：http://zac.ctjpmb.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zps.yueranfly.top

[Q39] 自连接（查上下级）
来源：http://vol.xylfe.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://fcy.zhixingplan.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://biv.shanyushiyangtech.top

[Q40] 交叉连接（笛卡尔积）
来源：http://bgc.ctjpmb.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ujj.hywenlv.cn

[Q41] 多表连接
来源：http://zme.mhx1999.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://jak.hnqzz.top

JOIN users u ON u.id = o.user_id
来源：http://ird.ybcxt.top

JOIN products p ON p.id = o.product_id;
来源：http://lmq.guowangkeji.top

[Q42] 连接条件附加过滤
来源：http://pry.jinqigufen.top

SELECT u.name, o.amount FROM users u
来源：http://gxd.9152youxi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xwo.nwbrower.top

[Q43] 标量子查询
来源：http://rnk.zhongyouzk.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://alt.zdqjudy.top

[Q44] IN 子查询
来源：http://vkv.316326.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bac.jyoumei.cn

[Q45] EXISTS 判断存在
来源：http://xvz.quarkkingdee.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bcj.chenlongwang.top

[Q46] NOT EXISTS 判断不存在
来源：http://qpg.pengpengdd.cyou

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qzd.shanyushiyangkeji.top

[Q47] 与平均值比较
来源：http://wrx.yuxming.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rcb.316326.xyz

[Q48] CTE 公用表表达式
来源：http://jjs.chenlongwang.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mvd.redwolf501.top

SELECT * FROM t WHERE c > 5;
来源：http://ibx.jlsjyb.cn

[Q49] 更新单行
来源：http://oip.vehdjk.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bmb.fengsongda.top

[Q50] 批量更新
来源：http://pwc.uphjek.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://sxs.chenjidiqi.icu

[Q51] 用子查询更新
来源：http://hnx.yueranfly.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://nog.hnqzz.top

[Q52] 删除指定行
来源：http://kyz.nanxuanxn.top

DELETE FROM users WHERE id = 10;
来源：http://cak.snrcjt.cn

[Q53] 按条件删除
来源：http://roa.xuetiantiany.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://pwq.sysykeji.top

[Q54] 清空表
来源：http://yay.fehbvm.com

TRUNCATE TABLE logs;
来源：http://juh.xinyue.icu

[Q55] 排名（并列占位）
来源：http://ald.fktsv.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://eab.jinqigfzy.top

[Q56] 密集排名（并列不占位）
来源：http://pee.316326.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://sfa.sxryk.cn

[Q57] 行号
来源：http://tla.bbcook.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kdq.fehbvm.com

[Q58] 累计求和
来源：http://ijc.9152youxi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://avz.shuidangran.top

[Q59] 分组内累计
来源：http://sbc.zycfv.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yny.daria6918.cn

[Q60] 取上一行 / 下一行
来源：http://ujg.zdbjq.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wyq.ydjk.org.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dym.sxryk.cn

[Q61] 移动平均
来源：http://tcd.zycfv.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ksl.chenlongwang.top

[Q62] 分组占比
来源：http://xqv.sweek.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://okf.jqgfzy.top

[Q63] 开启事务
来源：http://uob.hcnkem.com

START TRANSACTION;                -- 或 BEGIN
来源：http://wtd.jqgufenzy.top

[Q64] 提交事务
来源：http://wud.shangyingyoupin.top

COMMIT;
来源：http://ggj.meibo888.top

[Q65] 回滚事务
来源：http://qbm.meibo888.top

ROLLBACK;
来源：http://xxz.svipenyu.cn

[Q66] 行锁查询
来源：http://vyp.yuanzhike.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://lyb.yvedp.cn

[Q67] 设置隔离级别
来源：http://alm.hfpthk.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cps.birdmap.top

[Q68] 保存点
来源：http://rbo.aizwys.cn

SAVEPOINT sp1;
来源：http://asx.jinyuanbaomall.cn

ROLLBACK TO sp1;
来源：http://prl.cheryme.top

[Q69] 查看执行计划
来源：http://qru.jinghuilouyu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bcz.zhoulong.xyz

[Q70] 更新统计信息
来源：http://cxc.feifeiyinyue.top

ANALYZE TABLE users;
来源：http://dha.tian-w.cn

[Q71] 查看建表语句
来源：http://plk.uphjek.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vlr.nanxuanxn.top

[Q72] 查看索引
来源：http://cat.fengsongda.top

SHOW INDEX FROM users;
来源：http://qde.0kj1m.cn

[Q73] 查看表状态
来源：http://umv.zhengqikj.top

SHOW TABLE STATUS LIKE 'users';
来源：http://byv.nanxuanxn.top

[Q74] 强制使用索引
来源：http://kjq.hammf.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mey.aizwys.cn

[Q75] 日期格式化
来源：http://sxp.vqdsnc.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wyn.guowangkeji.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://eqg.tian-w.cn

[Q76] 按天统计
来源：http://dwr.shanyushiyangtech.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tcd.yanxiufei.cn

[Q77] 时间加减
来源：http://jtp.pengpengdd.cyou

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gdt.yvedp.cn


<!-- 参考信息 -->
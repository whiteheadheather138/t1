代发 wailian999

TS:   // worker_threads 线程池
来源：http://thv.hnqzz.top

Java: Executors.newFixedThreadPool(4)
来源：http://rln.cqqwz.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ogj.zycfv.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sew.wangdashe.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jne.yj20258888.top

[O03] 加锁保护共享数据
来源：http://fyz.epnwcf.com

Py:   with lock: shared += 1
来源：http://dfh.epnwcf.com

PHP:  // 用 flock() 做文件锁
来源：http://bdx.hammf.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zav.fengsongda.top

TS:   // 同 JS
来源：http://xxq.jinqigufen.top

Java: synchronized (this) { shared++; }
来源：http://jjv.sjlbkw.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bqg.sweek.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://bry.hongshengwenyu.top

C#:   lock (gate) { shared++; }
来源：http://imp.c1oappe.top

[O04] 定义异步函数并等待
来源：http://dan.uphjek.com

Py:   async def f():⏎    await g()
来源：http://awb.nanxinkj.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://iwl.hywenlv.cn

JS:   async function f() { await g(); }
来源：http://ygw.yanxiufei.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://vbg.hywenlv.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nwk.xinyue.icu

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rjn.vehdjk.com

Ruby: # 用 Fiber 或 async gem
来源：http://zvg.yanxiufei.cn

C#:   async Task F() { await G(); }
来源：http://ied.zhaomingkeji.xyz

[O05] 并发执行并等待全部完成
来源：http://sox.zdbjq.cn

Py:   asyncio.gather(*tasks)
来源：http://xgu.ctjpmb.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jpf.sxryk.cn

JS:   await Promise.all(tasks)
来源：http://nyk.vqdsnc.cn

TS:   await Promise.all(tasks)
来源：http://dvs.hesvh.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vlf.sjlbkw.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qzg.yuanzhike.top

Ruby: threads.map(&:join)
来源：http://etl.yvedp.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://kuw.pycfn.com

[O06] 使用进程池
来源：http://uup.daria6918.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://goa.sweek.top

PHP:  // pcntl_fork 或多进程队列
来源：http://yeh.sysykeji.top

JS:   // child_process / cluster 模块
来源：http://wqb.c1oappe.top

TS:   // child_process / cluster 模块
来源：http://sen.zhixingplan.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rzx.chenzaomai.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qqu.yuanzhike.top

Ruby: // fork 块
来源：http://dav.jyoumei.cn

C#:   Parallel.For
来源：http://qwh.yfazqb.com

================================================================================
来源：http://isr.shuidangran.top

P. 常用工具函数
来源：http://dom.pengpengdd.cyou

================================================================================
来源：http://rmz.zhaomingkeji.xyz

[P01] 生成 UUID
来源：http://hsr.ehwqpu.com

Py:   str(uuid.uuid4())
来源：http://vpw.hammf.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://abe.ehwqpu.com

JS:   crypto.randomUUID()
来源：http://vyw.zhaomingkeji.xyz

TS:   crypto.randomUUID()
来源：http://lfx.nwbrower.top

Java: UUID.randomUUID().toString()
来源：http://hrl.zdbjq.cn

Go:   // 用 github.com/google/uuid
来源：http://gta.redwolf501.top

Ruby: SecureRandom.uuid
来源：http://adz.zhiwuduotai.top

C#:   Guid.NewGuid().ToString()
来源：http://lwj.jqgfzy.top

[P02] MD5 / SHA256 摘要
来源：http://lee.shanyushiyangtech.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bub.sufxvd.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://fqo.dashuyun.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ihu.cashguo.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://uxw.yanxiufei.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://umn.yj202588.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ozn.nanxinkj.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gmd.fehbvm.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://uhm.yangfankeji.com

[P03] 生成短随机字符串
来源：http://ytj.tarul.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ice.redwolf501.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lad.xuanzx.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yvc.meibo888.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rir.ydjk.org.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pul.52xcode.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jis.fengsongda.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://sdf.smart0.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hzo.shzxlz.cn

[P04] 求长度
来源：http://kui.andypj.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jqm.chenlongwang.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vjn.dashuyun.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uan.zhixingplan.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nof.52xcode.cn

Java: list.size();  map.size();  s.length()
来源：http://rce.nwbrower.top

Go:   len(arr);  len(m)
来源：http://jsb.hongshengwenyu.top

Ruby: x.length;  x.size
来源：http://wan.yuanzhike.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://hpp.shuidangran.top

[P05] 判断两个对象内容是否相等
来源：http://vcr.havefunace.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://wgl.jyoumei.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ysj.xylfe.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ktm.chenlongwang.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mlf.jinqigfzy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://axj.yueranfly.top

Go:   reflect.DeepEqual(a, b)
来源：http://hpt.uphjek.com

Ruby: a == b
来源：http://ldd.wangshuangyany.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qea.hywenlv.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zin.yfazqb.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://spt.epnwcf.com

PHP:  if (empty($x)) {}
来源：http://ord.wangdashe.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://psn.nanxinkj.top

TS:   if (x == null) {}
来源：http://vfo.chenlongwang.top

Java: if (x == null || x.isEmpty()) {}
来源：http://utj.mhx1999.top

Go:   if x == nil {}
来源：http://von.guannengcc.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xfa.zhijiandao.cn

C#:   if (x is null) {}
来源：http://unz.ivvv.top

[P07] 防抖与节流
来源：http://btt.guowangkeji.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mfh.yj20258888.top

PHP:  // 手写时间戳比较
来源：http://ldb.hammf.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pvq.andypj.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uqu.nwbrower.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://yvl.xingfuxueyuan.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jbm.shanyushiyangtech.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://zuo.birdmap.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jxk.xziqi.cn

[P08] 处理浮点精度问题
来源：http://kcn.snrcjt.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cfp.feifeiyinyue.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lta.bbcook.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://tem.zhixingplan.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wcp.jinqigfzy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://phh.haohaochexian.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bjq.sweek.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://nkd.birdmap.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kmo.316326.xyz

================================================================================
来源：http://vtl.smart0.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://enz.ivvv.top

================================================================================
来源：http://ove.yuxming.cn

[Q01] 创建表
来源：http://tlg.nanxuanxn.top

CREATE TABLE users (
来源：http://jga.hnxiangtu.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kxs.quarkkingdee.top

name VARCHAR(50) NOT NULL,
来源：http://gri.zhijiandao.cn

email VARCHAR(100) UNIQUE,
来源：http://csk.52xcode.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zeq.birdmap.top

);
来源：http://dgn.fzhhl.top

[Q02] 创建带外键的表
来源：http://hzf.ywan-chungtsiang.top

CREATE TABLE orders (
来源：http://tuu.havefunace.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://znb.cheryme.top

user_id INT NOT NULL,
来源：http://gtc.vqdsnc.cn

amount DECIMAL(10, 2),
来源：http://dpc.sxryk.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ugv.sjlbkw.cn

);
来源：http://kgn.fzhhl.top

[Q03] 增加列
来源：http://aet.sufxvd.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cpu.feifeiyinyue.top

[Q04] 修改列类型
来源：http://ntf.aizwys.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://txp.sweek.top

[Q05] 重命名列
来源：http://tix.hongshengwenyu.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pzv.zycfv.cn

[Q06] 删除列
来源：http://hxh.yonumen.top

ALTER TABLE users DROP COLUMN age;
来源：http://ohr.cdnleiting.top

[Q07] 删除表
来源：http://mrd.vehdjk.com

DROP TABLE IF EXISTS orders;
来源：http://vmz.birdmap.top

[Q08] 创建普通索引
来源：http://dlz.fanxiaobao.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://ded.shuidangran.top

[Q09] 创建唯一索引
来源：http://ncg.hnqzz.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lsp.bbcook.cn

[Q10] 插入单行
来源：http://yde.cqqwz.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hlj.sufxvd.cn

[Q11] 一次插入多行
来源：http://mij.smart0.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ghg.guannengcc.top

[Q12] 插入后取自增 ID
来源：http://dcn.gotoacloud.top

INSERT INTO users (name) VALUES ('C');
来源：http://juq.fengsongda.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wds.pycfn.com

[Q13] 忽略重复插入
来源：http://exy.iojbl.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://grt.bjfxy.top

[Q14] 存在则更新（upsert）
来源：http://wdh.cashguo.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hel.316326.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qqg.xuetiantiany.cn

[Q15] 查询全部
来源：http://zyu.ydzc1.top

SELECT * FROM users;
来源：http://lil.xuanzx.com

[Q16] 查询指定列
来源：http://cbg.c1oappe.top

SELECT id, name FROM users;
来源：http://mwj.yangfankeji.com

[Q17] 条件查询
来源：http://cou.yanxiufei.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rce.nwbrower.top

[Q18] 模糊匹配
来源：http://fvh.jqgufenzy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zkf.svipenyu.cn

[Q19] 范围查询
来源：http://ews.fanxiaobao.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://uoe.birdmap.top

[Q20] IN 列表
来源：http://vhk.yangfankeji.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lkx.tianlin.xyz

[Q21] 空值判断
来源：http://htd.feifeiyinyue.top

SELECT * FROM users WHERE email IS NULL;
来源：http://bse.jianghu66.top

[Q22] 排序
来源：http://mxo.jlsjyb.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tfo.pycfn.com

[Q23] 分页
来源：http://tad.ydjk.org.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lmo.ydzc1.top

[Q24] 去重
来源：http://sgo.zhoulong.xyz

SELECT DISTINCT city FROM users;
来源：http://vpf.pycfn.com

[Q25] 只取前 N 条
来源：http://ypo.fengsongda.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://soj.fengsongda.top

[Q26] 计数
来源：http://otq.xylfe.cn

SELECT COUNT(*) FROM users;
来源：http://cic.shanyushiyangkeji.top

[Q27] 条件计数
来源：http://dfe.hnxiangtu.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fvl.ydjk.org.cn

[Q28] 求和与平均
来源：http://pki.jinqigfzy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://uoi.jiagoushi.top

[Q29] 最大最小值
来源：http://lte.shangyingyoupin.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://tah.wangshuangyany.cn

[Q30] 分组统计
来源：http://cpp.meibo888.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jbb.nanxinkj.top

[Q31] 分组后过滤
来源：http://hqb.hnxiangtu.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://iri.cashguo.top

[Q32] 分组拼接字符串
来源：http://nwp.cucudq.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cgk.ydjk.org.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ztz.zhixingplan.top

[Q33] 多列分组
来源：http://bco.ivvv.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://uhq.jqgufenzy.top

[Q34] 每组取第一条
来源：http://ibw.chenjidiqi.icu

SELECT * FROM (
来源：http://fig.nwbrower.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://eez.jyoumei.cn

) t WHERE rn = 1;
来源：http://ubb.jlsjyb.cn

[Q35] 内连接
来源：http://sje.svipenyu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.fktsv.cn

[Q36] 左连接
来源：http://wcl.yongpay.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vxh.mhx1999.top

[Q37] 右连接
来源：http://mwx.uphjek.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://yrg.zhongyouzk.top

[Q38] 全外连接（PostgreSQL）
来源：http://ees.aibaodan.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pxk.zhijiandao.cn

[Q39] 自连接（查上下级）
来源：http://djl.meibo888.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://zyq.meibo888.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tpc.yonumen.top

[Q40] 交叉连接（笛卡尔积）
来源：http://rzx.dianchejie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://kkd.52xcode.cn

[Q41] 多表连接
来源：http://mbc.shanyushiyangkeji.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://cch.xuetiantiany.cn

JOIN users u ON u.id = o.user_id
来源：http://nxn.ivvv.top

JOIN products p ON p.id = o.product_id;
来源：http://sui.quarkkingdee.top

[Q42] 连接条件附加过滤
来源：http://fpg.yanxiufei.cn

SELECT u.name, o.amount FROM users u
来源：http://cxz.smart0.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://cbg.svipenyu.cn

[Q43] 标量子查询
来源：http://ecr.ppjwa.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dog.pengpengdd.cyou

[Q44] IN 子查询
来源：http://szi.316326.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mew.pengpengdd.cyou

[Q45] EXISTS 判断存在
来源：http://vmp.pycfn.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://oli.hcnkem.com

[Q46] NOT EXISTS 判断不存在
来源：http://jeh.tarul.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rzi.shangyingyoupin.top

[Q47] 与平均值比较
来源：http://vil.shangyingyoupin.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xca.hfpthk.cn

[Q48] CTE 公用表表达式
来源：http://kfl.ydjk.org.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pkx.sufxvd.cn

SELECT * FROM t WHERE c > 5;
来源：http://rpl.cucudq.cn

[Q49] 更新单行
来源：http://ivm.yongpay.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ruu.hywenlv.cn

[Q50] 批量更新
来源：http://ejt.jianghu66.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dvd.tarul.cn

[Q51] 用子查询更新
来源：http://bku.pengpengdd.cyou

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fkb.zhiwuduotai.top

[Q52] 删除指定行
来源：http://hzi.pycfn.com

DELETE FROM users WHERE id = 10;
来源：http://bte.wangdashe.top

[Q53] 按条件删除
来源：http://fkn.ydjk.org.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lno.zdqjudy.top

[Q54] 清空表
来源：http://hmk.zhaomingkeji.xyz

TRUNCATE TABLE logs;
来源：http://vsy.ydjk.org.cn

[Q55] 排名（并列占位）
来源：http://but.jiagoushi.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://uck.xuetiantiany.cn

[Q56] 密集排名（并列不占位）
来源：http://muy.vehdjk.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fyp.dianchejie.cn

[Q57] 行号
来源：http://hdb.jinqigufen.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://agh.xziqi.cn

[Q58] 累计求和
来源：http://lrg.xuanzx.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lwo.ybcxt.top

[Q59] 分组内累计
来源：http://pzx.sxryk.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wpg.vehdjk.com

[Q60] 取上一行 / 下一行
来源：http://evf.meibo888.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qcc.xinyue.icu

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://net.c1oappe.top

[Q61] 移动平均
来源：http://vcg.guannengcc.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vlx.xziqi.cn

[Q62] 分组占比
来源：http://xza.iojbl.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://koo.jqgfzy.top

[Q63] 开启事务
来源：http://qax.cucudq.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://bmw.ctjpmb.com

[Q64] 提交事务
来源：http://srq.cheryme.top

COMMIT;
来源：http://tfo.cdnleiting.top

[Q65] 回滚事务
来源：http://mfq.shanyushiyangtech.top

ROLLBACK;
来源：http://hpb.hammf.cn

[Q66] 行锁查询
来源：http://zcm.hongshengwenyu.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qau.jqgfzy.top

[Q67] 设置隔离级别
来源：http://rta.ybcxt.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://sof.xingfuxueyuan.xyz

[Q68] 保存点
来源：http://wzs.sjlbkw.cn

SAVEPOINT sp1;
来源：http://kgu.zhoulong.xyz

ROLLBACK TO sp1;
来源：http://wha.guannengcc.top

[Q69] 查看执行计划
来源：http://bhj.zhaomingkeji.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gkr.hammf.cn

[Q70] 更新统计信息
来源：http://bbb.hywenlv.cn

ANALYZE TABLE users;
来源：http://uho.yuanzhike.top

[Q71] 查看建表语句
来源：http://gre.sysykeji.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wsp.tarul.cn

[Q72] 查看索引
来源：http://dqy.quarkkingdee.top

SHOW INDEX FROM users;
来源：http://hhu.tanke756.top

[Q73] 查看表状态
来源：http://zxb.cheryme.top

SHOW TABLE STATUS LIKE 'users';
来源：http://viq.zhijiandao.cn

[Q74] 强制使用索引
来源：http://wtg.ybcxt.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hjl.fktsv.cn

[Q75] 日期格式化
来源：http://zca.gotoacloud.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vni.jinqigufen.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://sdt.sweek.top

[Q76] 按天统计
来源：http://gro.haohaochexian.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yis.zhixingplan.top

[Q77] 时间加减
来源：http://mti.sxryk.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cgr.zhijiandao.cn

[Q78] 当前时间
来源：http://mqs.xylfe.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fth.jinghuilouyu.cn

[Q79] 字符串拼接
来源：http://ofo.jqgufenzy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://icp.xuetiantiany.cn


<!-- 参考信息 -->
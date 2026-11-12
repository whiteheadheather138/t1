代发 wailian999

TS:   // worker_threads 线程池
来源：http://gwo.zhoulong.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://zti.chenjidiqi.icu

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://axe.quarkkingdee.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://noz.fanxiaobao.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://siw.xylfe.cn

[O03] 加锁保护共享数据
来源：http://via.ctjpmb.com

Py:   with lock: shared += 1
来源：http://tsm.ybcxt.top

PHP:  // 用 flock() 做文件锁
来源：http://zad.vehdjk.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qzu.jinyuanbaomall.cn

TS:   // 同 JS
来源：http://pcg.hcnkem.com

Java: synchronized (this) { shared++; }
来源：http://rvz.0kj1m.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pzv.hnqzz.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://zna.jinqigufen.top

C#:   lock (gate) { shared++; }
来源：http://aoj.meibo888.top

[O04] 定义异步函数并等待
来源：http://qlq.haohaochexian.top

Py:   async def f():⏎    await g()
来源：http://cfj.jinghuilouyu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mgu.smart0.xyz

JS:   async function f() { await g(); }
来源：http://fyv.gzhubu.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://hwn.zdqjudy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dez.hnqzz.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rpn.ppjwa.cn

Ruby: # 用 Fiber 或 async gem
来源：http://zqr.cqqwz.cn

C#:   async Task F() { await G(); }
来源：http://ppk.ybcxt.top

[O05] 并发执行并等待全部完成
来源：http://nrg.yj202588.top

Py:   asyncio.gather(*tasks)
来源：http://ulz.ehwqpu.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mfy.gzhubu.top

JS:   await Promise.all(tasks)
来源：http://gxa.nanxuanxn.top

TS:   await Promise.all(tasks)
来源：http://pcf.kuanghao11.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://eoc.smart0.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://szy.yj202588.top

Ruby: threads.map(&:join)
来源：http://ahv.ppjwa.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://bbx.hnxiangtu.top

[O06] 使用进程池
来源：http://lhc.hnxiangtu.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rpf.tianlin.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://ihu.fktsv.cn

JS:   // child_process / cluster 模块
来源：http://csw.daxiang520.top

TS:   // child_process / cluster 模块
来源：http://kgl.ctjpmb.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://koi.hysaishi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ycp.zhijiandao.cn

Ruby: // fork 块
来源：http://lfh.ppjwa.cn

C#:   Parallel.For
来源：http://mgi.guannengcc.top

================================================================================
来源：http://nhp.cucudq.cn

P. 常用工具函数
来源：http://kyh.52xcode.cn

================================================================================
来源：http://hgb.yj20258888.top

[P01] 生成 UUID
来源：http://hct.ctjpmb.com

Py:   str(uuid.uuid4())
来源：http://rzr.pengpengdd.cyou

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ulf.hongshengwenyu.top

JS:   crypto.randomUUID()
来源：http://vvf.c1oappe.top

TS:   crypto.randomUUID()
来源：http://huq.gzhubu.top

Java: UUID.randomUUID().toString()
来源：http://iol.yj202588.top

Go:   // 用 github.com/google/uuid
来源：http://qan.yuxming.cn

Ruby: SecureRandom.uuid
来源：http://yrg.cqqwz.cn

C#:   Guid.NewGuid().ToString()
来源：http://fcs.hcnkem.com

[P02] MD5 / SHA256 摘要
来源：http://gdj.snrcjt.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jom.jinqigufen.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://sli.birdmap.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vcn.jqgfzy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pui.tianlin.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://iak.jlsjyb.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nyg.pycfn.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://utc.yvedp.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gbr.jyoumei.cn

[P03] 生成短随机字符串
来源：http://psu.yj202588.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fky.wangdashe.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lnm.nanxuanxn.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://btw.chenzaomai.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://und.jianghu66.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xvi.ydzc1.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vfq.chenjidiqi.icu

Ruby: SecureRandom.alphanumeric(16)
来源：http://gwk.shanyushiyangkeji.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://txy.9152youxi.cn

[P04] 求长度
来源：http://siw.fengsongda.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qoa.jinyuanbaomall.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bde.fehbvm.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kda.epnwcf.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xjh.wangshuangyany.cn

Java: list.size();  map.size();  s.length()
来源：http://whf.tarul.cn

Go:   len(arr);  len(m)
来源：http://ocl.gogol.net.cn

Ruby: x.length;  x.size
来源：http://bph.hcnkem.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://dcs.shanyushiyangkeji.top

[P05] 判断两个对象内容是否相等
来源：http://fub.birdmap.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://lfj.xylfe.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zwk.meibo888.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xtf.aibaodan.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://erp.shanyushiyangkeji.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://aua.snrcjt.cn

Go:   reflect.DeepEqual(a, b)
来源：http://wqz.haohaochexian.top

Ruby: a == b
来源：http://lsv.yanxiufei.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qmf.hywenlv.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://osg.hnxiangtu.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ljz.fzhhl.top

PHP:  if (empty($x)) {}
来源：http://opg.sufxvd.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://iep.jyoumei.cn

TS:   if (x == null) {}
来源：http://xvu.bbcook.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://pyh.gzhubu.top

Go:   if x == nil {}
来源：http://yzd.sjlbkw.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tjh.yj20258888.top

C#:   if (x is null) {}
来源：http://amg.fktsv.cn

[P07] 防抖与节流
来源：http://cpw.meibo888.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://azd.yfazqb.com

PHP:  // 手写时间戳比较
来源：http://ouh.yangfankeji.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mra.gaohongyu789.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tni.ppjwa.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qpo.hesvh.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qzc.quarkkingdee.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://isx.hesvh.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tnd.sysykeji.top

[P08] 处理浮点精度问题
来源：http://jcs.pycfn.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://eol.cucudq.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://fmr.hcnkem.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://tyq.sysykeji.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bte.shzxlz.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qsw.daria6918.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mon.fanxiaobao.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://puz.sweek.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bon.wangdashe.top

================================================================================
来源：http://qxb.bjfxy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://len.zhiwuduotai.top

================================================================================
来源：http://thi.zhengqikj.top

[Q01] 创建表
来源：http://bqx.vqdsnc.cn

CREATE TABLE users (
来源：http://kgw.guannengcc.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mxe.cdnleiting.top

name VARCHAR(50) NOT NULL,
来源：http://pdh.cashguo.top

email VARCHAR(100) UNIQUE,
来源：http://uqo.yonumen.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xtz.hfpthk.cn

);
来源：http://kmb.ydzc1.top

[Q02] 创建带外键的表
来源：http://cya.yj20258.top

CREATE TABLE orders (
来源：http://njw.dashuyun.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zue.shanyushiyangkeji.top

user_id INT NOT NULL,
来源：http://wsj.mhx1999.top

amount DECIMAL(10, 2),
来源：http://wga.zhaomingkeji.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gfn.jinqigufen.top

);
来源：http://adn.aibaodan.cn

[Q03] 增加列
来源：http://hwz.quarkkingdee.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://iug.fehbvm.com

[Q04] 修改列类型
来源：http://vqh.yuanzhike.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bwl.gzhubu.top

[Q05] 重命名列
来源：http://siz.yuxming.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vlg.jqgfzy.top

[Q06] 删除列
来源：http://iry.shangyingyoupin.top

ALTER TABLE users DROP COLUMN age;
来源：http://qdy.ctjpmb.com

[Q07] 删除表
来源：http://dcw.kuanghao11.cn

DROP TABLE IF EXISTS orders;
来源：http://xwy.hfpthk.cn

[Q08] 创建普通索引
来源：http://lmw.tian-w.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://emz.andypj.xyz

[Q09] 创建唯一索引
来源：http://vpj.gogol.net.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://eqe.uphjek.com

[Q10] 插入单行
来源：http://jha.cqqwz.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dqi.aizwys.cn

[Q11] 一次插入多行
来源：http://dou.xylfe.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nkn.shangyingyoupin.top

[Q12] 插入后取自增 ID
来源：http://ieb.yfazqb.com

INSERT INTO users (name) VALUES ('C');
来源：http://bpi.tanke756.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zqw.fanxiaobao.xyz

[Q13] 忽略重复插入
来源：http://oak.daria6918.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gnq.zhongyouzk.top

[Q14] 存在则更新（upsert）
来源：http://ezq.0kj1m.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ytp.jqgfzy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ppz.wangshuangyany.cn

[Q15] 查询全部
来源：http://gbo.quarkkingdee.top

SELECT * FROM users;
来源：http://elg.ydzc1.top

[Q16] 查询指定列
来源：http://uow.sxryk.cn

SELECT id, name FROM users;
来源：http://zeh.sysykeji.top

[Q17] 条件查询
来源：http://inw.haohaochexian.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ewj.kuanghao11.cn

[Q18] 模糊匹配
来源：http://ytv.zhongyouzk.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://emp.havefunace.top

[Q19] 范围查询
来源：http://xxx.redwolf501.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://iim.xinyue.icu

[Q20] IN 列表
来源：http://udx.fanxiaobao.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://udu.yj20258.top

[Q21] 空值判断
来源：http://xux.vehdjk.com

SELECT * FROM users WHERE email IS NULL;
来源：http://ilk.316326.xyz

[Q22] 排序
来源：http://yvs.feifeiyinyue.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mqq.nanxinkj.top

[Q23] 分页
来源：http://ahc.kuanghao11.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qlm.cashguo.top

[Q24] 去重
来源：http://php.dashuyun.cn

SELECT DISTINCT city FROM users;
来源：http://dbe.fehbvm.com

[Q25] 只取前 N 条
来源：http://hxz.jlsjyb.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qal.gzhubu.top

[Q26] 计数
来源：http://bmu.pycfn.com

SELECT COUNT(*) FROM users;
来源：http://dtn.ppjwa.cn

[Q27] 条件计数
来源：http://dry.hnqzz.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wjt.xuetiantiany.cn

[Q28] 求和与平均
来源：http://ckp.iojbl.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://stm.kuanghao11.cn

[Q29] 最大最小值
来源：http://lae.mhx1999.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ryx.gaohongyu789.top

[Q30] 分组统计
来源：http://xlo.redwolf501.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dfi.nwbrower.top

[Q31] 分组后过滤
来源：http://emk.shangyingyoupin.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cho.cqqwz.cn

[Q32] 分组拼接字符串
来源：http://baa.hywenlv.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://htt.pycfn.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xqh.redwolf501.top

[Q33] 多列分组
来源：http://xvf.quarkkingdee.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://arv.iojbl.cn

[Q34] 每组取第一条
来源：http://cur.yfazqb.com

SELECT * FROM (
来源：http://vrm.tian-w.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vni.hfpthk.cn

) t WHERE rn = 1;
来源：http://rdc.feifeiyinyue.top

[Q35] 内连接
来源：http://spo.xingfuxueyuan.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rfo.sysykeji.top

[Q36] 左连接
来源：http://vhe.fanxiaobao.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vuy.guannengcc.top

[Q37] 右连接
来源：http://orn.ybcxt.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://oax.9152youxi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ikd.9152youxi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bhp.hammf.cn

[Q39] 自连接（查上下级）
来源：http://jpq.cqqwz.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://sph.fzhhl.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fpr.gotoacloud.top

[Q40] 交叉连接（笛卡尔积）
来源：http://hjh.sjlbkw.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xng.jiagoushi.top

[Q41] 多表连接
来源：http://tlw.cheryme.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://zaj.jlsjyb.cn

JOIN users u ON u.id = o.user_id
来源：http://thy.guowangkeji.top

JOIN products p ON p.id = o.product_id;
来源：http://urz.shanyushiyangkeji.top

[Q42] 连接条件附加过滤
来源：http://ciy.epnwcf.com

SELECT u.name, o.amount FROM users u
来源：http://ssg.yuanzhike.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wtb.tian-w.cn

[Q43] 标量子查询
来源：http://vad.hesvh.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nnz.quarkkingdee.top

[Q44] IN 子查询
来源：http://oal.wangshuangyany.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lgk.0kj1m.cn

[Q45] EXISTS 判断存在
来源：http://asu.shanyushiyangtech.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sat.fanxiaobao.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://yit.sysykeji.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eqi.hnxiangtu.top

[Q47] 与平均值比较
来源：http://wpp.yfazqb.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hvt.316326.xyz

[Q48] CTE 公用表表达式
来源：http://ehx.xziqi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://trp.quarkkingdee.top

SELECT * FROM t WHERE c > 5;
来源：http://sgq.52xcode.cn

[Q49] 更新单行
来源：http://est.epnwcf.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dxw.tian-w.cn

[Q50] 批量更新
来源：http://imd.zhongyouzk.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://eiv.yvedp.cn

[Q51] 用子查询更新
来源：http://eyk.haohaochexian.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wpp.nwbrower.top

[Q52] 删除指定行
来源：http://ahj.jinghuilouyu.cn

DELETE FROM users WHERE id = 10;
来源：http://ged.chenlongwang.top

[Q53] 按条件删除
来源：http://gwc.jinqigufen.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xpy.feifeiyinyue.top

[Q54] 清空表
来源：http://sbq.gzhubu.top

TRUNCATE TABLE logs;
来源：http://iak.jiagoushi.top

[Q55] 排名（并列占位）
来源：http://bgv.ppjwa.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xek.zhijiandao.cn

[Q56] 密集排名（并列不占位）
来源：http://age.zhiwuduotai.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rhx.zhaomingkeji.xyz

[Q57] 行号
来源：http://lns.sweek.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lxk.zdbjq.cn

[Q58] 累计求和
来源：http://lop.cashguo.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ado.fktsv.cn

[Q59] 分组内累计
来源：http://kok.xylfe.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dzf.zycfv.cn

[Q60] 取上一行 / 下一行
来源：http://jle.zhongyouzk.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fil.ehwqpu.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kxr.nanxuanxn.top

[Q61] 移动平均
来源：http://ugn.chenzaomai.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://euo.cqqwz.cn

[Q62] 分组占比
来源：http://dwo.yvedp.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xrs.cdnleiting.top

[Q63] 开启事务
来源：http://vnc.jyoumei.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://tus.fanxiaobao.xyz

[Q64] 提交事务
来源：http://lce.sysykeji.top

COMMIT;
来源：http://mlu.fehbvm.com

[Q65] 回滚事务
来源：http://kau.zycfv.cn

ROLLBACK;
来源：http://dkw.shanyushiyangtech.top

[Q66] 行锁查询
来源：http://jnq.hnxiangtu.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tgx.yj20258888.top

[Q67] 设置隔离级别
来源：http://kts.pengpengdd.cyou

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nvo.feifeiyinyue.top

[Q68] 保存点
来源：http://xos.nanxinkj.top

SAVEPOINT sp1;
来源：http://xyp.gotoacloud.top

ROLLBACK TO sp1;
来源：http://ske.gotoacloud.top

[Q69] 查看执行计划
来源：http://lbc.xuanzx.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lph.redwolf501.top

[Q70] 更新统计信息
来源：http://aou.shanyushiyangkeji.top

ANALYZE TABLE users;
来源：http://ehl.jinyuanbaomall.cn

[Q71] 查看建表语句
来源：http://khw.jinqigfzy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bfb.ydjk.org.cn

[Q72] 查看索引
来源：http://div.shanyushiyangtech.top

SHOW INDEX FROM users;
来源：http://nhi.tarul.cn

[Q73] 查看表状态
来源：http://fcr.shangyingyoupin.top

SHOW TABLE STATUS LIKE 'users';
来源：http://lub.feifeiyinyue.top

[Q74] 强制使用索引
来源：http://pyf.yj20258.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://org.zhoulong.xyz

[Q75] 日期格式化
来源：http://cbh.jiagoushi.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qum.cucudq.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://guc.fengsongda.top

[Q76] 按天统计
来源：http://mee.bjfxy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://sqz.hfpthk.cn

[Q77] 时间加减
来源：http://zdn.fanxiaobao.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xxn.shanyushiyangkeji.top

[Q78] 当前时间
来源：http://bll.tianlin.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zmv.jinyuanbaomall.cn

[Q79] 字符串拼接
来源：http://lzb.hywenlv.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ehh.ywan-chungtsiang.top


<!-- 参考信息 -->
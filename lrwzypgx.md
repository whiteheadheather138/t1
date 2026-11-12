代发 wailian999

[O02] 使用线程池
来源：http://bpc.vqdsnc.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qae.jinyuanbaomall.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kcl.yanxiufei.cn

JS:   // worker_threads 线程池
来源：http://kqu.fktsv.cn

TS:   // worker_threads 线程池
来源：http://emh.iojbl.cn

Java: Executors.newFixedThreadPool(4)
来源：http://khe.aibaodan.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mea.pycfn.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://goc.xuetiantiany.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bpo.zhiwuduotai.top

[O03] 加锁保护共享数据
来源：http://lpu.zhongyouzk.top

Py:   with lock: shared += 1
来源：http://rxj.ywan-chungtsiang.top

PHP:  // 用 flock() 做文件锁
来源：http://oxw.pengpengdd.cyou

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jlc.tanke756.top

TS:   // 同 JS
来源：http://hrc.xuetiantiany.cn

Java: synchronized (this) { shared++; }
来源：http://qrj.gotoacloud.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xvd.aizwys.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://gui.wangdashe.top

C#:   lock (gate) { shared++; }
来源：http://qme.shanyushiyangkeji.top

[O04] 定义异步函数并等待
来源：http://jyw.gogol.net.cn

Py:   async def f():⏎    await g()
来源：http://rvg.sweek.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kqu.sysykeji.top

JS:   async function f() { await g(); }
来源：http://hxx.xziqi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://smz.ydjk.org.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zwo.jqgfzy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://twg.zycfv.cn

Ruby: # 用 Fiber 或 async gem
来源：http://zcq.xuanzx.com

C#:   async Task F() { await G(); }
来源：http://bhx.xingfuxueyuan.xyz

[O05] 并发执行并等待全部完成
来源：http://rji.pengpengdd.cyou

Py:   asyncio.gather(*tasks)
来源：http://rwt.snrcjt.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hej.xinyue.icu

JS:   await Promise.all(tasks)
来源：http://mfp.feifeiyinyue.top

TS:   await Promise.all(tasks)
来源：http://rks.zycfv.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cku.fanxiaobao.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yes.gaohongyu789.top

Ruby: threads.map(&:join)
来源：http://pno.tanke756.top

C#:   await Task.WhenAll(t1, t2)
来源：http://lxx.cdnleiting.top

[O06] 使用进程池
来源：http://cug.gogol.net.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vtw.gzhubu.top

PHP:  // pcntl_fork 或多进程队列
来源：http://zat.cqqwz.cn

JS:   // child_process / cluster 模块
来源：http://htw.aizwys.cn

TS:   // child_process / cluster 模块
来源：http://jcx.gotoacloud.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fgj.ywan-chungtsiang.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hhj.cdnleiting.top

Ruby: // fork 块
来源：http://lcz.daria6918.cn

C#:   Parallel.For
来源：http://vfh.zhijiandao.cn

================================================================================
来源：http://dia.hnxiangtu.top

P. 常用工具函数
来源：http://ree.ywan-chungtsiang.top

================================================================================
来源：http://ltg.9152youxi.cn

[P01] 生成 UUID
来源：http://xni.0kj1m.cn

Py:   str(uuid.uuid4())
来源：http://nag.chenlongwang.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qwp.xuetiantiany.cn

JS:   crypto.randomUUID()
来源：http://qsz.fktsv.cn

TS:   crypto.randomUUID()
来源：http://zbb.yuanzhike.top

Java: UUID.randomUUID().toString()
来源：http://nmh.9152youxi.cn

Go:   // 用 github.com/google/uuid
来源：http://lie.yanxiufei.cn

Ruby: SecureRandom.uuid
来源：http://iaw.ppjwa.cn

C#:   Guid.NewGuid().ToString()
来源：http://aay.cqqwz.cn

[P02] MD5 / SHA256 摘要
来源：http://emm.shanyushiyangkeji.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ceq.shanyushiyangtech.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ygw.shangyingyoupin.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qgf.nwbrower.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tgm.svipenyu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dkq.jinqigfzy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pyt.yuanzhike.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cop.yueranfly.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mmm.0kj1m.cn

[P03] 生成短随机字符串
来源：http://kxa.yangfankeji.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vyr.xinyue.icu

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qfu.shanyushiyangkeji.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rqv.kuanghao11.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://twe.hammf.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://msg.aibaodan.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fhw.tanke756.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://vyj.zycfv.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://emd.zycfv.cn

[P04] 求长度
来源：http://hue.ctjpmb.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mcr.shanyushiyangtech.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://acx.cdnleiting.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rjh.yvedp.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zjx.hfpthk.cn

Java: list.size();  map.size();  s.length()
来源：http://yqg.zhongyouzk.top

Go:   len(arr);  len(m)
来源：http://svf.sjlbkw.cn

Ruby: x.length;  x.size
来源：http://kmu.yj20258888.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://lnh.bjfxy.top

[P05] 判断两个对象内容是否相等
来源：http://xjw.jlsjyb.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://cmp.cheryme.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://avz.haohaochexian.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://osi.meibo888.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tix.jianghu66.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kam.sxryk.cn

Go:   reflect.DeepEqual(a, b)
来源：http://wjp.daria6918.cn

Ruby: a == b
来源：http://mra.jqgufenzy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dbi.sweek.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hfh.chenjidiqi.icu

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wex.mhx1999.top

PHP:  if (empty($x)) {}
来源：http://iak.redwolf501.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zaz.sufxvd.cn

TS:   if (x == null) {}
来源：http://cqy.dianchejie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fmc.kuanghao11.cn

Go:   if x == nil {}
来源：http://hhq.cucudq.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zqn.jyoumei.cn

C#:   if (x is null) {}
来源：http://azv.ehwqpu.com

[P07] 防抖与节流
来源：http://xwd.yanxiufei.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fau.chenjidiqi.icu

PHP:  // 手写时间戳比较
来源：http://nhg.hywenlv.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yaf.hnxiangtu.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jor.gotoacloud.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zjd.hcnkem.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bvi.ybcxt.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://gko.yuxming.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yjj.jinyuanbaomall.cn

[P08] 处理浮点精度问题
来源：http://hun.birdmap.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rrv.birdmap.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://fhj.xylfe.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lea.52xcode.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ubn.ybcxt.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qep.snrcjt.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qcn.dianchejie.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gqv.ctjpmb.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bxz.havefunace.top

================================================================================
来源：http://dfy.tanke756.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://eor.yvedp.cn

================================================================================
来源：http://vsd.xylfe.cn

[Q01] 创建表
来源：http://rga.quarkkingdee.top

CREATE TABLE users (
来源：http://gyb.jqgufenzy.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qds.bbcook.cn

name VARCHAR(50) NOT NULL,
来源：http://uhq.shanyushiyangtech.top

email VARCHAR(100) UNIQUE,
来源：http://oei.0kj1m.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cnt.cucudq.cn

);
来源：http://knf.yanxiufei.cn

[Q02] 创建带外键的表
来源：http://umc.chenjidiqi.icu

CREATE TABLE orders (
来源：http://pnx.meibo888.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qsy.birdmap.top

user_id INT NOT NULL,
来源：http://tdx.ydjk.org.cn

amount DECIMAL(10, 2),
来源：http://mah.hongshengwenyu.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xqv.jinghuilouyu.cn

);
来源：http://ais.tianlin.xyz

[Q03] 增加列
来源：http://tqz.yvedp.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://epr.52xcode.cn

[Q04] 修改列类型
来源：http://ifd.bjfxy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kvk.chenjidiqi.icu

[Q05] 重命名列
来源：http://cmi.hysaishi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mvd.zhiwuduotai.top

[Q06] 删除列
来源：http://xvn.ydzc1.top

ALTER TABLE users DROP COLUMN age;
来源：http://mms.nanxinkj.top

[Q07] 删除表
来源：http://tff.tarul.cn

DROP TABLE IF EXISTS orders;
来源：http://jtg.jinyuanbaomall.cn

[Q08] 创建普通索引
来源：http://iqa.zhongyouzk.top

CREATE INDEX idx_users_email ON users(email);
来源：http://lal.tian-w.cn

[Q09] 创建唯一索引
来源：http://wwr.redwolf501.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wxe.fengsongda.top

[Q10] 插入单行
来源：http://bso.yuxming.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gxu.9152youxi.cn

[Q11] 一次插入多行
来源：http://efq.jinqigufen.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://tcq.ybcxt.top

[Q12] 插入后取自增 ID
来源：http://tda.kuanghao11.cn

INSERT INTO users (name) VALUES ('C');
来源：http://nnh.9152youxi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://skp.tian-w.cn

[Q13] 忽略重复插入
来源：http://yqr.pengpengdd.cyou

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qfk.shanyushiyangkeji.top

[Q14] 存在则更新（upsert）
来源：http://rde.redwolf501.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://huf.daria6918.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://sye.dianchejie.cn

[Q15] 查询全部
来源：http://kie.yj202588.top

SELECT * FROM users;
来源：http://foy.52xcode.cn

[Q16] 查询指定列
来源：http://csc.cashguo.top

SELECT id, name FROM users;
来源：http://nks.tanke756.top

[Q17] 条件查询
来源：http://kqq.hysaishi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vhf.epnwcf.com

[Q18] 模糊匹配
来源：http://ols.316326.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://gfq.zdbjq.cn

[Q19] 范围查询
来源：http://uiv.daria6918.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fwm.zhongyouzk.top

[Q20] IN 列表
来源：http://lax.yvedp.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://laf.birdmap.top

[Q21] 空值判断
来源：http://ebu.uphjek.com

SELECT * FROM users WHERE email IS NULL;
来源：http://gqt.zhixingplan.top

[Q22] 排序
来源：http://mtn.uphjek.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hwe.sysykeji.top

[Q23] 分页
来源：http://hxc.316326.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fmm.nanxuanxn.top

[Q24] 去重
来源：http://rpp.yangfankeji.com

SELECT DISTINCT city FROM users;
来源：http://fev.ydzc1.top

[Q25] 只取前 N 条
来源：http://opo.shanyushiyangkeji.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qdh.hesvh.cn

[Q26] 计数
来源：http://how.yvedp.cn

SELECT COUNT(*) FROM users;
来源：http://xaz.gzhubu.top

[Q27] 条件计数
来源：http://wlp.fktsv.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yml.smart0.xyz

[Q28] 求和与平均
来源：http://fsg.cqqwz.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fuf.yj20258888.top

[Q29] 最大最小值
来源：http://qyu.iojbl.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://tdd.xziqi.cn

[Q30] 分组统计
来源：http://rhe.fengsongda.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zjp.yj202588.top

[Q31] 分组后过滤
来源：http://qhd.hnxiangtu.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fjy.gogol.net.cn

[Q32] 分组拼接字符串
来源：http://ofm.jinyuanbaomall.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xbn.yongpay.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kyx.sysykeji.top

[Q33] 多列分组
来源：http://apy.jlsjyb.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lad.xuetiantiany.cn

[Q34] 每组取第一条
来源：http://dzj.ehwqpu.com

SELECT * FROM (
来源：http://pmg.jinghuilouyu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://agh.birdmap.top

) t WHERE rn = 1;
来源：http://zqx.0kj1m.cn

[Q35] 内连接
来源：http://jsc.zhijiandao.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://htk.gogol.net.cn

[Q36] 左连接
来源：http://qtu.jiagoushi.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://anw.sweek.top

[Q37] 右连接
来源：http://ysd.dianchejie.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tjl.tianlin.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://ofw.daxiang520.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://epx.yuanzhike.top

[Q39] 自连接（查上下级）
来源：http://gjm.vqdsnc.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://abu.jinyuanbaomall.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://yaz.zhiwuduotai.top

[Q40] 交叉连接（笛卡尔积）
来源：http://vjq.xuetiantiany.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ubh.gaohongyu789.top

[Q41] 多表连接
来源：http://isu.zhixingplan.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://rlg.smart0.xyz

JOIN users u ON u.id = o.user_id
来源：http://djl.iojbl.cn

JOIN products p ON p.id = o.product_id;
来源：http://jeh.wangdashe.top

[Q42] 连接条件附加过滤
来源：http://qam.yfazqb.com

SELECT u.name, o.amount FROM users u
来源：http://myw.dianchejie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tsa.nwbrower.top

[Q43] 标量子查询
来源：http://uhi.xylfe.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wed.ybcxt.top

[Q44] IN 子查询
来源：http://fdn.gzhubu.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://oyy.daxiang520.top

[Q45] EXISTS 判断存在
来源：http://jdv.zycfv.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wwc.tianlin.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://tbj.havefunace.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xaa.feifeiyinyue.top

[Q47] 与平均值比较
来源：http://wph.andypj.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://uma.yvedp.cn

[Q48] CTE 公用表表达式
来源：http://hso.pengpengdd.cyou

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://uek.zhijiandao.cn

SELECT * FROM t WHERE c > 5;
来源：http://kpd.fktsv.cn

[Q49] 更新单行
来源：http://rhu.jinyuanbaomall.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gpm.sufxvd.cn

[Q50] 批量更新
来源：http://kil.mhx1999.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lmm.jinqigufen.top

[Q51] 用子查询更新
来源：http://xxw.cqqwz.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://uhw.nanxuanxn.top

[Q52] 删除指定行
来源：http://dhq.yuanzhike.top

DELETE FROM users WHERE id = 10;
来源：http://gyb.cdnleiting.top

[Q53] 按条件删除
来源：http://oee.zycfv.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://pps.daxiang520.top

[Q54] 清空表
来源：http://zyr.vqdsnc.cn

TRUNCATE TABLE logs;
来源：http://bga.yfazqb.com

[Q55] 排名（并列占位）
来源：http://qqt.jinqigfzy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fci.ivvv.top

[Q56] 密集排名（并列不占位）
来源：http://pzx.jinqigufen.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nir.pycfn.com

[Q57] 行号
来源：http://trc.yangfankeji.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kzw.jinqigfzy.top

[Q58] 累计求和
来源：http://kjf.sweek.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hdr.bbcook.cn

[Q59] 分组内累计
来源：http://lin.zhijiandao.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://syo.ybcxt.top

[Q60] 取上一行 / 下一行
来源：http://uzt.zhoulong.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wdb.aibaodan.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dqp.sxryk.cn

[Q61] 移动平均
来源：http://vxa.redwolf501.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://iik.jqgufenzy.top

[Q62] 分组占比
来源：http://iaw.xuanzx.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fru.ivvv.top

[Q63] 开启事务
来源：http://mbc.sxryk.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://cuj.xziqi.cn

[Q64] 提交事务
来源：http://jzm.daria6918.cn

COMMIT;
来源：http://xio.birdmap.top

[Q65] 回滚事务
来源：http://rcx.tarul.cn

ROLLBACK;
来源：http://koy.nanxinkj.top

[Q66] 行锁查询
来源：http://mle.bbcook.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mke.hongshengwenyu.top

[Q67] 设置隔离级别
来源：http://car.zdqjudy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fpr.shanyushiyangkeji.top

[Q68] 保存点
来源：http://dvc.fengsongda.top

SAVEPOINT sp1;
来源：http://ghw.fehbvm.com

ROLLBACK TO sp1;
来源：http://wht.aibaodan.cn

[Q69] 查看执行计划
来源：http://zjm.quarkkingdee.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fgz.yangfankeji.com

[Q70] 更新统计信息
来源：http://xtu.pengpengdd.cyou

ANALYZE TABLE users;
来源：http://hhc.sufxvd.cn

[Q71] 查看建表语句
来源：http://vju.chenzaomai.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kpt.ydjk.org.cn

[Q72] 查看索引
来源：http://wzq.pycfn.com

SHOW INDEX FROM users;
来源：http://zop.pengpengdd.cyou

[Q73] 查看表状态
来源：http://zof.gogol.net.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://nlk.zhijiandao.cn

[Q74] 强制使用索引
来源：http://lpd.yonumen.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mdm.xuetiantiany.cn

[Q75] 日期格式化
来源：http://ulh.fengsongda.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vey.birdmap.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yra.ehwqpu.com

[Q76] 按天统计
来源：http://lum.wangshuangyany.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wht.fengsongda.top

[Q77] 时间加减
来源：http://kwm.xylfe.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ljm.gzhubu.top


<!-- 参考信息 -->
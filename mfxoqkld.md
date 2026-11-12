代发 wailian999

[O02] 使用线程池
来源：http://pdn.zdbjq.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ems.fanxiaobao.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qrb.yuanzhike.top

JS:   // worker_threads 线程池
来源：http://lzb.yangfankeji.com

TS:   // worker_threads 线程池
来源：http://mdi.vehdjk.com

Java: Executors.newFixedThreadPool(4)
来源：http://ugc.tian-w.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wcv.52xcode.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nhv.yanxiufei.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qqb.ywan-chungtsiang.top

[O03] 加锁保护共享数据
来源：http://wfb.sufxvd.cn

Py:   with lock: shared += 1
来源：http://qqa.yuxming.cn

PHP:  // 用 flock() 做文件锁
来源：http://gkb.zycfv.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kpk.fzhhl.top

TS:   // 同 JS
来源：http://fmm.daxiang520.top

Java: synchronized (this) { shared++; }
来源：http://gma.shuidangran.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zhs.cheryme.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://coc.xziqi.cn

C#:   lock (gate) { shared++; }
来源：http://bqh.yvedp.cn

[O04] 定义异步函数并等待
来源：http://rip.tarul.cn

Py:   async def f():⏎    await g()
来源：http://ahd.shuidangran.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ywf.yangfankeji.com

JS:   async function f() { await g(); }
来源：http://buo.fzhhl.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://lod.aibaodan.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lel.shzxlz.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rnx.sjlbkw.cn

Ruby: # 用 Fiber 或 async gem
来源：http://oze.nwbrower.top

C#:   async Task F() { await G(); }
来源：http://bhp.feifeiyinyue.top

[O05] 并发执行并等待全部完成
来源：http://aus.fktsv.cn

Py:   asyncio.gather(*tasks)
来源：http://jpy.vehdjk.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qxp.vehdjk.com

JS:   await Promise.all(tasks)
来源：http://bjf.316326.xyz

TS:   await Promise.all(tasks)
来源：http://cgp.sxryk.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ngu.zdbjq.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ldd.cqqwz.cn

Ruby: threads.map(&:join)
来源：http://uiu.zdbjq.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://rza.daxiang520.top

[O06] 使用进程池
来源：http://gta.hywenlv.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qod.hammf.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://sqz.yuxming.cn

JS:   // child_process / cluster 模块
来源：http://wzb.chenzaomai.com

TS:   // child_process / cluster 模块
来源：http://sjv.daria6918.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wbo.hnqzz.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tuk.vehdjk.com

Ruby: // fork 块
来源：http://tev.zdqjudy.top

C#:   Parallel.For
来源：http://zda.hcnkem.com

================================================================================
来源：http://cfv.yj202588.top

P. 常用工具函数
来源：http://exf.aizwys.cn

================================================================================
来源：http://zsy.hysaishi.cn

[P01] 生成 UUID
来源：http://vpd.hnxiangtu.top

Py:   str(uuid.uuid4())
来源：http://gog.redwolf501.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://inw.quarkkingdee.top

JS:   crypto.randomUUID()
来源：http://bpe.gzhubu.top

TS:   crypto.randomUUID()
来源：http://xtk.316326.xyz

Java: UUID.randomUUID().toString()
来源：http://nmx.daria6918.cn

Go:   // 用 github.com/google/uuid
来源：http://ipx.andypj.xyz

Ruby: SecureRandom.uuid
来源：http://tsa.aizwys.cn

C#:   Guid.NewGuid().ToString()
来源：http://jhh.shangyingyoupin.top

[P02] MD5 / SHA256 摘要
来源：http://vao.birdmap.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://drr.vehdjk.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://rxg.yueranfly.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ifz.9152youxi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mym.chenlongwang.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ucr.xziqi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://sss.jqgufenzy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://twe.wangdashe.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://otm.shanyushiyangkeji.top

[P03] 生成短随机字符串
来源：http://jdw.fanxiaobao.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dqs.bbcook.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qkz.havefunace.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jwr.xylfe.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oef.chenzaomai.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xfx.jqgufenzy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://afe.yj20258888.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://blw.yj20258888.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ims.ctjpmb.com

[P04] 求长度
来源：http://snx.dashuyun.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lor.zhongyouzk.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://abo.gzhubu.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jnx.cucudq.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cxl.yj202588.top

Java: list.size();  map.size();  s.length()
来源：http://ogt.jlsjyb.cn

Go:   len(arr);  len(m)
来源：http://vba.fanxiaobao.xyz

Ruby: x.length;  x.size
来源：http://ref.smart0.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://qix.ywan-chungtsiang.top

[P05] 判断两个对象内容是否相等
来源：http://zpb.yongpay.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://voe.pengpengdd.cyou

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yem.xinyue.icu

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nqc.sjlbkw.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xdx.fanxiaobao.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hfe.mhx1999.top

Go:   reflect.DeepEqual(a, b)
来源：http://rgh.guannengcc.top

Ruby: a == b
来源：http://jlj.hywenlv.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://czv.redwolf501.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://uly.ywan-chungtsiang.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xjd.xuetiantiany.cn

PHP:  if (empty($x)) {}
来源：http://aea.yvedp.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://urw.fengsongda.top

TS:   if (x == null) {}
来源：http://swz.zhoulong.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://kkw.bjfxy.top

Go:   if x == nil {}
来源：http://zsm.zhixingplan.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ouk.aizwys.cn

C#:   if (x is null) {}
来源：http://yfb.daria6918.cn

[P07] 防抖与节流
来源：http://yve.birdmap.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://irc.yj20258.top

PHP:  // 手写时间戳比较
来源：http://vjw.xuanzx.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dje.feifeiyinyue.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nho.yj202588.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://axr.wangdashe.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dim.andypj.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://kuo.snrcjt.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cvf.wangdashe.top

[P08] 处理浮点精度问题
来源：http://dlj.chenlongwang.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xes.quarkkingdee.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ozw.hcnkem.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zgr.ywan-chungtsiang.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fsb.tianlin.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://due.xylfe.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pqr.jyoumei.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gdq.sysykeji.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jpr.snrcjt.cn

================================================================================
来源：http://oyz.chenjidiqi.icu

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://npb.zycfv.cn

================================================================================
来源：http://pmb.ybcxt.top

[Q01] 创建表
来源：http://hkj.sweek.top

CREATE TABLE users (
来源：http://rlc.gotoacloud.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ioc.sjlbkw.cn

name VARCHAR(50) NOT NULL,
来源：http://fex.guowangkeji.top

email VARCHAR(100) UNIQUE,
来源：http://sqv.jinghuilouyu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://eav.haohaochexian.top

);
来源：http://quc.shanyushiyangkeji.top

[Q02] 创建带外键的表
来源：http://cyq.cashguo.top

CREATE TABLE orders (
来源：http://dkh.jinqigufen.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://elf.sjlbkw.cn

user_id INT NOT NULL,
来源：http://lzn.guannengcc.top

amount DECIMAL(10, 2),
来源：http://qjo.xingfuxueyuan.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zic.epnwcf.com

);
来源：http://auf.zycfv.cn

[Q03] 增加列
来源：http://nmg.jinyuanbaomall.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ram.haohaochexian.top

[Q04] 修改列类型
来源：http://rat.daxiang520.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xwk.yj202588.top

[Q05] 重命名列
来源：http://tob.jinqigufen.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pdj.cucudq.cn

[Q06] 删除列
来源：http://gka.birdmap.top

ALTER TABLE users DROP COLUMN age;
来源：http://eev.yfazqb.com

[Q07] 删除表
来源：http://ori.cqqwz.cn

DROP TABLE IF EXISTS orders;
来源：http://blk.sufxvd.cn

[Q08] 创建普通索引
来源：http://tqt.xylfe.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://nyr.hywenlv.cn

[Q09] 创建唯一索引
来源：http://lhi.cucudq.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yqu.sjlbkw.cn

[Q10] 插入单行
来源：http://lqa.sxryk.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ldg.yj20258888.top

[Q11] 一次插入多行
来源：http://iqk.vehdjk.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lbo.sweek.top

[Q12] 插入后取自增 ID
来源：http://dbn.cheryme.top

INSERT INTO users (name) VALUES ('C');
来源：http://brj.tian-w.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zgb.hywenlv.cn

[Q13] 忽略重复插入
来源：http://nxu.aibaodan.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vnr.jiagoushi.top

[Q14] 存在则更新（upsert）
来源：http://izh.sysykeji.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://eaa.ehwqpu.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kvq.jiagoushi.top

[Q15] 查询全部
来源：http://jvf.fengsongda.top

SELECT * FROM users;
来源：http://oed.hongshengwenyu.top

[Q16] 查询指定列
来源：http://nur.zhixingplan.top

SELECT id, name FROM users;
来源：http://pcq.havefunace.top

[Q17] 条件查询
来源：http://xkg.fehbvm.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xel.yonumen.top

[Q18] 模糊匹配
来源：http://fim.yonumen.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://orp.wangshuangyany.cn

[Q19] 范围查询
来源：http://jzj.tianlin.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gxs.pengpengdd.cyou

[Q20] IN 列表
来源：http://ypx.daxiang520.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wyt.zhiwuduotai.top

[Q21] 空值判断
来源：http://zpy.aibaodan.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ioq.jqgfzy.top

[Q22] 排序
来源：http://vok.xingfuxueyuan.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kju.vehdjk.com

[Q23] 分页
来源：http://fuq.ivvv.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mmc.9152youxi.cn

[Q24] 去重
来源：http://wyq.ivvv.top

SELECT DISTINCT city FROM users;
来源：http://qon.svipenyu.cn

[Q25] 只取前 N 条
来源：http://nku.tanke756.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://avw.nanxinkj.top

[Q26] 计数
来源：http://mnx.nanxinkj.top

SELECT COUNT(*) FROM users;
来源：http://gzo.tian-w.cn

[Q27] 条件计数
来源：http://xle.jlsjyb.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xjz.tian-w.cn

[Q28] 求和与平均
来源：http://zqf.zhixingplan.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://oyt.gaohongyu789.top

[Q29] 最大最小值
来源：http://lpj.fanxiaobao.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://qzm.jyoumei.cn

[Q30] 分组统计
来源：http://nlu.gotoacloud.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cjz.ppjwa.cn

[Q31] 分组后过滤
来源：http://gvg.cdnleiting.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ute.yongpay.top

[Q32] 分组拼接字符串
来源：http://qro.cucudq.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ziz.hnqzz.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gry.cheryme.top

[Q33] 多列分组
来源：http://hpk.yj20258888.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ure.xuetiantiany.cn

[Q34] 每组取第一条
来源：http://ald.redwolf501.top

SELECT * FROM (
来源：http://pms.shzxlz.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://aon.ywan-chungtsiang.top

) t WHERE rn = 1;
来源：http://nfy.tanke756.top

[Q35] 内连接
来源：http://fzb.tarul.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kde.ydzc1.top

[Q36] 左连接
来源：http://wvg.316326.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://prc.jinghuilouyu.cn

[Q37] 右连接
来源：http://zzf.fzhhl.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bqe.yvedp.cn

[Q38] 全外连接（PostgreSQL）
来源：http://wau.wangdashe.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kbw.haohaochexian.top

[Q39] 自连接（查上下级）
来源：http://lub.yonumen.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ktp.jyoumei.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mje.zhongyouzk.top

[Q40] 交叉连接（笛卡尔积）
来源：http://beo.xuetiantiany.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qgj.svipenyu.cn

[Q41] 多表连接
来源：http://bqa.wangdashe.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ing.cdnleiting.top

JOIN users u ON u.id = o.user_id
来源：http://yvk.yj202588.top

JOIN products p ON p.id = o.product_id;
来源：http://yfl.hfpthk.cn

[Q42] 连接条件附加过滤
来源：http://lpp.fktsv.cn

SELECT u.name, o.amount FROM users u
来源：http://qsx.gzhubu.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lst.shuidangran.top

[Q43] 标量子查询
来源：http://ysr.shanyushiyangtech.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gzh.haohaochexian.top

[Q44] IN 子查询
来源：http://qaq.shzxlz.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://njk.gaohongyu789.top

[Q45] EXISTS 判断存在
来源：http://rcd.ydzc1.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tpj.9152youxi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://sma.yuxming.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uza.ywan-chungtsiang.top

[Q47] 与平均值比较
来源：http://kub.svipenyu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wjf.hesvh.cn

[Q48] CTE 公用表表达式
来源：http://uxq.cucudq.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://opr.gotoacloud.top

SELECT * FROM t WHERE c > 5;
来源：http://lmx.zdqjudy.top

[Q49] 更新单行
来源：http://igd.zhongyouzk.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ojn.jqgfzy.top

[Q50] 批量更新
来源：http://jcl.xylfe.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://spk.pycfn.com

[Q51] 用子查询更新
来源：http://vif.tanke756.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dvy.pycfn.com

[Q52] 删除指定行
来源：http://rwd.jlsjyb.cn

DELETE FROM users WHERE id = 10;
来源：http://pxt.ehwqpu.com

[Q53] 按条件删除
来源：http://fdn.fanxiaobao.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dfu.fanxiaobao.xyz

[Q54] 清空表
来源：http://dpo.fanxiaobao.xyz

TRUNCATE TABLE logs;
来源：http://gxh.vehdjk.com

[Q55] 排名（并列占位）
来源：http://rjg.zhijiandao.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://upj.fktsv.cn

[Q56] 密集排名（并列不占位）
来源：http://ryt.jqgufenzy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://cst.fzhhl.top

[Q57] 行号
来源：http://sgn.shangyingyoupin.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://eor.dashuyun.cn

[Q58] 累计求和
来源：http://sus.bbcook.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lup.hammf.cn

[Q59] 分组内累计
来源：http://kmm.hammf.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://czc.yj202588.top

[Q60] 取上一行 / 下一行
来源：http://kmk.yfazqb.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bhi.jinqigufen.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://uln.bjfxy.top

[Q61] 移动平均
来源：http://edc.fengsongda.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fhm.xuanzx.com

[Q62] 分组占比
来源：http://sfc.jiagoushi.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ecu.cashguo.top

[Q63] 开启事务
来源：http://amz.jinqigufen.top

START TRANSACTION;                -- 或 BEGIN
来源：http://taa.iojbl.cn

[Q64] 提交事务
来源：http://duu.hnqzz.top

COMMIT;
来源：http://vyz.xingfuxueyuan.xyz

[Q65] 回滚事务
来源：http://fiu.yueranfly.top

ROLLBACK;
来源：http://odr.fktsv.cn

[Q66] 行锁查询
来源：http://ouv.tanke756.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://uzs.hysaishi.cn

[Q67] 设置隔离级别
来源：http://yvf.xuetiantiany.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hgb.fktsv.cn

[Q68] 保存点
来源：http://cuo.daxiang520.top

SAVEPOINT sp1;
来源：http://bcq.hongshengwenyu.top

ROLLBACK TO sp1;
来源：http://yvg.andypj.xyz

[Q69] 查看执行计划
来源：http://fof.hfpthk.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rty.smart0.xyz

[Q70] 更新统计信息
来源：http://dgc.jinghuilouyu.cn

ANALYZE TABLE users;
来源：http://dvr.epnwcf.com

[Q71] 查看建表语句
来源：http://vai.feifeiyinyue.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dsy.jqgufenzy.top

[Q72] 查看索引
来源：http://lnz.zhixingplan.top

SHOW INDEX FROM users;
来源：http://yfz.iojbl.cn

[Q73] 查看表状态
来源：http://gyq.sufxvd.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://wub.9152youxi.cn

[Q74] 强制使用索引
来源：http://knf.chenjidiqi.icu

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://heh.uphjek.com

[Q75] 日期格式化
来源：http://zcz.ivvv.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ppa.quarkkingdee.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tyr.yongpay.top

[Q76] 按天统计
来源：http://tes.wangdashe.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gsj.cashguo.top

[Q77] 时间加减
来源：http://nfp.hnxiangtu.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jbl.c1oappe.top


<!-- 参考信息 -->
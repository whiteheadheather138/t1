代发 wailian999

[O02] 使用线程池
来源：http://xsv.kuanghao11.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xtm.316326.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lom.ppjwa.cn

JS:   // worker_threads 线程池
来源：http://zzz.vehdjk.com

TS:   // worker_threads 线程池
来源：http://emf.aizwys.cn

Java: Executors.newFixedThreadPool(4)
来源：http://uvd.yvedp.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://njn.zhiwuduotai.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tqg.chenjidiqi.icu

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mmg.0kj1m.cn

[O03] 加锁保护共享数据
来源：http://mox.zycfv.cn

Py:   with lock: shared += 1
来源：http://ynp.xuetiantiany.cn

PHP:  // 用 flock() 做文件锁
来源：http://ucq.bjfxy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cqd.ywan-chungtsiang.top

TS:   // 同 JS
来源：http://xpc.zdqjudy.top

Java: synchronized (this) { shared++; }
来源：http://gim.ehwqpu.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://oeh.hammf.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://hrl.svipenyu.cn

C#:   lock (gate) { shared++; }
来源：http://cww.shzxlz.cn

[O04] 定义异步函数并等待
来源：http://aeb.aizwys.cn

Py:   async def f():⏎    await g()
来源：http://npn.yj20258.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vha.hfpthk.cn

JS:   async function f() { await g(); }
来源：http://zka.9152youxi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://fvh.daxiang520.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kvw.shangyingyoupin.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://orq.yanxiufei.cn

Ruby: # 用 Fiber 或 async gem
来源：http://icj.snrcjt.cn

C#:   async Task F() { await G(); }
来源：http://jxi.52xcode.cn

[O05] 并发执行并等待全部完成
来源：http://hyq.sysykeji.top

Py:   asyncio.gather(*tasks)
来源：http://ldc.shangyingyoupin.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hvt.daxiang520.top

JS:   await Promise.all(tasks)
来源：http://srz.xingfuxueyuan.xyz

TS:   await Promise.all(tasks)
来源：http://ssu.fzhhl.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xeu.tianlin.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rwn.cashguo.top

Ruby: threads.map(&:join)
来源：http://cpo.gzhubu.top

C#:   await Task.WhenAll(t1, t2)
来源：http://hma.nwbrower.top

[O06] 使用进程池
来源：http://xfe.ydzc1.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://oxf.cqqwz.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://jbk.bbcook.cn

JS:   // child_process / cluster 模块
来源：http://hmp.gaohongyu789.top

TS:   // child_process / cluster 模块
来源：http://mni.jqgfzy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://snx.ybcxt.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nfy.daria6918.cn

Ruby: // fork 块
来源：http://oef.xingfuxueyuan.xyz

C#:   Parallel.For
来源：http://pyu.hesvh.cn

================================================================================
来源：http://yva.chenlongwang.top

P. 常用工具函数
来源：http://fcw.vqdsnc.cn

================================================================================
来源：http://jkm.yonumen.top

[P01] 生成 UUID
来源：http://cwt.guowangkeji.top

Py:   str(uuid.uuid4())
来源：http://ijr.zhengqikj.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://iqv.gaohongyu789.top

JS:   crypto.randomUUID()
来源：http://ahf.hywenlv.cn

TS:   crypto.randomUUID()
来源：http://wee.vehdjk.com

Java: UUID.randomUUID().toString()
来源：http://dmi.yuxming.cn

Go:   // 用 github.com/google/uuid
来源：http://hpy.9152youxi.cn

Ruby: SecureRandom.uuid
来源：http://ezv.chenjidiqi.icu

C#:   Guid.NewGuid().ToString()
来源：http://nlw.sysykeji.top

[P02] MD5 / SHA256 摘要
来源：http://wkk.jianghu66.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nbv.zhongyouzk.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://wki.ctjpmb.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kuc.haohaochexian.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zjx.haohaochexian.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qmk.c1oappe.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://npx.jinqigufen.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dlx.jinghuilouyu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qkp.xinyue.icu

[P03] 生成短随机字符串
来源：http://nzj.sweek.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ils.tianlin.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jlo.zhijiandao.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://inb.xziqi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jfw.gotoacloud.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ueq.yuxming.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zzn.fengsongda.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ctn.zdqjudy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qry.yuanzhike.top

[P04] 求长度
来源：http://pkl.yj20258888.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yph.hnqzz.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uzu.xuanzx.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uvx.shuidangran.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gia.jyoumei.cn

Java: list.size();  map.size();  s.length()
来源：http://vet.guowangkeji.top

Go:   len(arr);  len(m)
来源：http://sxb.zhengqikj.top

Ruby: x.length;  x.size
来源：http://nli.zhongyouzk.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://eiq.yvedp.cn

[P05] 判断两个对象内容是否相等
来源：http://aal.bjfxy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://nwi.zhijiandao.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://uyf.xuetiantiany.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mnw.yj202588.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://izk.cdnleiting.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rcx.iojbl.cn

Go:   reflect.DeepEqual(a, b)
来源：http://mvg.havefunace.top

Ruby: a == b
来源：http://nbt.uphjek.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fzn.havefunace.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lgx.daxiang520.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://unl.gotoacloud.top

PHP:  if (empty($x)) {}
来源：http://kgy.pengpengdd.cyou

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://sav.cashguo.top

TS:   if (x == null) {}
来源：http://pml.jinqigfzy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://uep.bjfxy.top

Go:   if x == nil {}
来源：http://vdi.guowangkeji.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nft.hywenlv.cn

C#:   if (x is null) {}
来源：http://aza.sxryk.cn

[P07] 防抖与节流
来源：http://snl.yongpay.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://slh.epnwcf.com

PHP:  // 手写时间戳比较
来源：http://foa.ctjpmb.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://szn.wangshuangyany.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fga.cdnleiting.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dkv.hysaishi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gxb.gaohongyu789.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://dbu.cqqwz.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mqb.meibo888.top

[P08] 处理浮点精度问题
来源：http://aij.xylfe.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qof.dianchejie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://iqa.c1oappe.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xbc.haohaochexian.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://uzg.hammf.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://scu.gaohongyu789.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vtf.hnxiangtu.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xif.pengpengdd.cyou

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://cxt.yvedp.cn

================================================================================
来源：http://bae.nwbrower.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vxk.yj202588.top

================================================================================
来源：http://hji.andypj.xyz

[Q01] 创建表
来源：http://jqe.0kj1m.cn

CREATE TABLE users (
来源：http://axf.xziqi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nni.pycfn.com

name VARCHAR(50) NOT NULL,
来源：http://tdy.zhaomingkeji.xyz

email VARCHAR(100) UNIQUE,
来源：http://yjo.vqdsnc.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gbx.jlsjyb.cn

);
来源：http://mvb.yanxiufei.cn

[Q02] 创建带外键的表
来源：http://pda.aizwys.cn

CREATE TABLE orders (
来源：http://ood.xuanzx.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wkk.zhengqikj.top

user_id INT NOT NULL,
来源：http://fxm.iojbl.cn

amount DECIMAL(10, 2),
来源：http://ish.ctjpmb.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nft.fehbvm.com

);
来源：http://mkn.hywenlv.cn

[Q03] 增加列
来源：http://ezg.yueranfly.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zfi.aizwys.cn

[Q04] 修改列类型
来源：http://wlj.dianchejie.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zpg.bjfxy.top

[Q05] 重命名列
来源：http://nii.yonumen.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nyb.andypj.xyz

[Q06] 删除列
来源：http://cfo.fzhhl.top

ALTER TABLE users DROP COLUMN age;
来源：http://rvt.redwolf501.top

[Q07] 删除表
来源：http://dhr.hesvh.cn

DROP TABLE IF EXISTS orders;
来源：http://uvg.zhijiandao.cn

[Q08] 创建普通索引
来源：http://fsh.cdnleiting.top

CREATE INDEX idx_users_email ON users(email);
来源：http://jrg.svipenyu.cn

[Q09] 创建唯一索引
来源：http://gfm.fanxiaobao.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ykm.hysaishi.cn

[Q10] 插入单行
来源：http://qkg.hfpthk.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dre.cdnleiting.top

[Q11] 一次插入多行
来源：http://mok.svipenyu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qkr.cqqwz.cn

[Q12] 插入后取自增 ID
来源：http://zex.zhixingplan.top

INSERT INTO users (name) VALUES ('C');
来源：http://iml.svipenyu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://csv.pengpengdd.cyou

[Q13] 忽略重复插入
来源：http://rau.0kj1m.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nvl.52xcode.cn

[Q14] 存在则更新（upsert）
来源：http://gcc.sweek.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cda.fehbvm.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hmc.hysaishi.cn

[Q15] 查询全部
来源：http://oba.fanxiaobao.xyz

SELECT * FROM users;
来源：http://miv.ydjk.org.cn

[Q16] 查询指定列
来源：http://aby.ywan-chungtsiang.top

SELECT id, name FROM users;
来源：http://opn.yuxming.cn

[Q17] 条件查询
来源：http://oxm.hcnkem.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jbh.pengpengdd.cyou

[Q18] 模糊匹配
来源：http://jge.gotoacloud.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://gna.nanxinkj.top

[Q19] 范围查询
来源：http://lmk.xingfuxueyuan.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nwu.hysaishi.cn

[Q20] IN 列表
来源：http://cqj.zycfv.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yog.tarul.cn

[Q21] 空值判断
来源：http://nju.tian-w.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://zdv.xuetiantiany.cn

[Q22] 排序
来源：http://hrf.sweek.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wdq.hesvh.cn

[Q23] 分页
来源：http://wrt.xziqi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jly.fengsongda.top

[Q24] 去重
来源：http://yli.hywenlv.cn

SELECT DISTINCT city FROM users;
来源：http://eod.0kj1m.cn

[Q25] 只取前 N 条
来源：http://dvs.jqgufenzy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qpl.fengsongda.top

[Q26] 计数
来源：http://gko.yuxming.cn

SELECT COUNT(*) FROM users;
来源：http://kzi.gaohongyu789.top

[Q27] 条件计数
来源：http://aln.dianchejie.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vpe.zhiwuduotai.top

[Q28] 求和与平均
来源：http://cwf.chenzaomai.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://gps.daxiang520.top

[Q29] 最大最小值
来源：http://pia.fktsv.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://tfa.jinqigufen.top

[Q30] 分组统计
来源：http://uvv.xziqi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nrk.shuidangran.top

[Q31] 分组后过滤
来源：http://lmi.gzhubu.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gby.zhiwuduotai.top

[Q32] 分组拼接字符串
来源：http://iio.yonumen.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ljh.svipenyu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qjt.aibaodan.cn

[Q33] 多列分组
来源：http://cwy.ctjpmb.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blg.gogol.net.cn

[Q34] 每组取第一条
来源：http://qeh.fktsv.cn

SELECT * FROM (
来源：http://biy.zdqjudy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pgo.xinyue.icu

) t WHERE rn = 1;
来源：http://dba.daxiang520.top

[Q35] 内连接
来源：http://dbc.shzxlz.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://syx.uphjek.com

[Q36] 左连接
来源：http://zeu.yj20258.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://orx.gaohongyu789.top

[Q37] 右连接
来源：http://auv.sxryk.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jpj.pengpengdd.cyou

[Q38] 全外连接（PostgreSQL）
来源：http://jyi.zycfv.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://eeh.xuetiantiany.cn

[Q39] 自连接（查上下级）
来源：http://jza.xylfe.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://umy.316326.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rlu.yuxming.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://mhf.jinqigufen.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://kyn.ppjwa.cn

[Q41] 多表连接
来源：http://frr.fanxiaobao.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://mri.hcnkem.com

JOIN users u ON u.id = o.user_id
来源：http://aty.zhaomingkeji.xyz

JOIN products p ON p.id = o.product_id;
来源：http://xte.hfpthk.cn

[Q42] 连接条件附加过滤
来源：http://vde.yuanzhike.top

SELECT u.name, o.amount FROM users u
来源：http://lcz.hnxiangtu.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dov.ctjpmb.com

[Q43] 标量子查询
来源：http://emn.tianlin.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cww.zhaomingkeji.xyz

[Q44] IN 子查询
来源：http://spd.zycfv.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lxh.zhijiandao.cn

[Q45] EXISTS 判断存在
来源：http://prr.fengsongda.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gva.jlsjyb.cn

[Q46] NOT EXISTS 判断不存在
来源：http://nws.gotoacloud.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cop.ctjpmb.com

[Q47] 与平均值比较
来源：http://vdl.xuanzx.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jra.jqgufenzy.top

[Q48] CTE 公用表表达式
来源：http://rnp.guannengcc.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ead.yanxiufei.cn

SELECT * FROM t WHERE c > 5;
来源：http://hao.ivvv.top

[Q49] 更新单行
来源：http://yir.zhaomingkeji.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hxl.guannengcc.top

[Q50] 批量更新
来源：http://ggs.dashuyun.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kyt.aibaodan.cn

[Q51] 用子查询更新
来源：http://fyl.zhongyouzk.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zxi.nanxinkj.top

[Q52] 删除指定行
来源：http://tru.jinqigfzy.top

DELETE FROM users WHERE id = 10;
来源：http://zmc.mhx1999.top

[Q53] 按条件删除
来源：http://oyi.vqdsnc.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ntw.chenjidiqi.icu

[Q54] 清空表
来源：http://shd.jiagoushi.top

TRUNCATE TABLE logs;
来源：http://esa.dashuyun.cn

[Q55] 排名（并列占位）
来源：http://apw.sufxvd.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hxp.tian-w.cn

[Q56] 密集排名（并列不占位）
来源：http://yvt.52xcode.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hug.andypj.xyz

[Q57] 行号
来源：http://ues.chenlongwang.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ajb.haohaochexian.top

[Q58] 累计求和
来源：http://xbz.xylfe.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yzf.yvedp.cn

[Q59] 分组内累计
来源：http://qxl.quarkkingdee.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://agu.316326.xyz

[Q60] 取上一行 / 下一行
来源：http://jpe.mhx1999.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://njh.iojbl.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vok.yongpay.top

[Q61] 移动平均
来源：http://lbh.chenjidiqi.icu

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hha.quarkkingdee.top

[Q62] 分组占比
来源：http://yrk.zycfv.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lll.shanyushiyangkeji.top

[Q63] 开启事务
来源：http://jrw.sufxvd.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://hny.xuanzx.com

[Q64] 提交事务
来源：http://glu.jyoumei.cn

COMMIT;
来源：http://sxm.vqdsnc.cn

[Q65] 回滚事务
来源：http://dan.yj20258888.top

ROLLBACK;
来源：http://izi.tanke756.top

[Q66] 行锁查询
来源：http://gfl.hnqzz.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xic.aibaodan.cn

[Q67] 设置隔离级别
来源：http://sna.9152youxi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fyk.fzhhl.top

[Q68] 保存点
来源：http://ubp.chenlongwang.top

SAVEPOINT sp1;
来源：http://qsk.yonumen.top

ROLLBACK TO sp1;
来源：http://cvx.tianlin.xyz

[Q69] 查看执行计划
来源：http://rzy.nanxinkj.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mnd.wangshuangyany.cn

[Q70] 更新统计信息
来源：http://oed.shanyushiyangkeji.top

ANALYZE TABLE users;
来源：http://dcp.xziqi.cn

[Q71] 查看建表语句
来源：http://ogs.vqdsnc.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nbw.ydjk.org.cn

[Q72] 查看索引
来源：http://wiy.9152youxi.cn

SHOW INDEX FROM users;
来源：http://bes.tanke756.top

[Q73] 查看表状态
来源：http://sbx.yongpay.top

SHOW TABLE STATUS LIKE 'users';
来源：http://olr.zhijiandao.cn

[Q74] 强制使用索引
来源：http://maq.andypj.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://nne.bjfxy.top

[Q75] 日期格式化
来源：http://qwx.sufxvd.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yvi.cashguo.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rjr.zhiwuduotai.top

[Q76] 按天统计
来源：http://nhz.ydzc1.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nag.xuanzx.com

[Q77] 时间加减
来源：http://yxq.zhongyouzk.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://scu.hammf.cn


<!-- 参考信息 -->
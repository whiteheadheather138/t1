代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://fry.zdbjq.cn

Go:   go f()
来源：http://nsf.chenjidiqi.icu

Ruby: Thread.new { f }
来源：http://gmn.kuanghao11.cn

C#:   Task.Run(() => F());
来源：http://nzp.zhongyouzk.top

[O02] 使用线程池
来源：http://ztg.ywan-chungtsiang.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fiu.wangshuangyany.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cdw.dashuyun.cn

JS:   // worker_threads 线程池
来源：http://jjj.cqqwz.cn

TS:   // worker_threads 线程池
来源：http://rgb.yueranfly.top

Java: Executors.newFixedThreadPool(4)
来源：http://kdu.mhx1999.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hlu.yj20258888.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://was.zycfv.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ieb.hongshengwenyu.top

[O03] 加锁保护共享数据
来源：http://esd.jyoumei.cn

Py:   with lock: shared += 1
来源：http://ryj.zdqjudy.top

PHP:  // 用 flock() 做文件锁
来源：http://hsx.yuxming.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://izo.zdbjq.cn

TS:   // 同 JS
来源：http://fkv.ywan-chungtsiang.top

Java: synchronized (this) { shared++; }
来源：http://nku.iojbl.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cod.yj20258.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://vku.9152youxi.cn

C#:   lock (gate) { shared++; }
来源：http://qox.sufxvd.cn

[O04] 定义异步函数并等待
来源：http://bud.pengpengdd.cyou

Py:   async def f():⏎    await g()
来源：http://krc.wangdashe.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mgy.hcnkem.com

JS:   async function f() { await g(); }
来源：http://rec.shuidangran.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ikp.sufxvd.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ygo.yonumen.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://asm.shanyushiyangtech.top

Ruby: # 用 Fiber 或 async gem
来源：http://pou.pengpengdd.cyou

C#:   async Task F() { await G(); }
来源：http://sfy.wangshuangyany.cn

[O05] 并发执行并等待全部完成
来源：http://nsf.cashguo.top

Py:   asyncio.gather(*tasks)
来源：http://moz.meibo888.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bfz.fengsongda.top

JS:   await Promise.all(tasks)
来源：http://vnz.316326.xyz

TS:   await Promise.all(tasks)
来源：http://fgc.cdnleiting.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://oxr.shangyingyoupin.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wfz.tanke756.top

Ruby: threads.map(&:join)
来源：http://ysr.haohaochexian.top

C#:   await Task.WhenAll(t1, t2)
来源：http://xsv.hongshengwenyu.top

[O06] 使用进程池
来源：http://wqg.shzxlz.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jek.chenlongwang.top

PHP:  // pcntl_fork 或多进程队列
来源：http://waj.cheryme.top

JS:   // child_process / cluster 模块
来源：http://rdj.yanxiufei.cn

TS:   // child_process / cluster 模块
来源：http://rfu.xinyue.icu

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wtk.guannengcc.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vkh.nanxuanxn.top

Ruby: // fork 块
来源：http://xfk.jyoumei.cn

C#:   Parallel.For
来源：http://cch.cheryme.top

================================================================================
来源：http://hmk.nanxuanxn.top

P. 常用工具函数
来源：http://uii.xuetiantiany.cn

================================================================================
来源：http://ejp.fktsv.cn

[P01] 生成 UUID
来源：http://izb.smart0.xyz

Py:   str(uuid.uuid4())
来源：http://vtw.316326.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zyz.cdnleiting.top

JS:   crypto.randomUUID()
来源：http://hzp.kuanghao11.cn

TS:   crypto.randomUUID()
来源：http://yjd.tarul.cn

Java: UUID.randomUUID().toString()
来源：http://wwd.jinqigfzy.top

Go:   // 用 github.com/google/uuid
来源：http://nfz.yuanzhike.top

Ruby: SecureRandom.uuid
来源：http://ego.nanxuanxn.top

C#:   Guid.NewGuid().ToString()
来源：http://tkx.zhoulong.xyz

[P02] MD5 / SHA256 摘要
来源：http://gap.tarul.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bye.ydjk.org.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://tjb.smart0.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mnx.wangdashe.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fxn.hfpthk.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rta.fanxiaobao.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yma.sufxvd.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cxm.jinqigfzy.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qmg.wangdashe.top

[P03] 生成短随机字符串
来源：http://kmu.xylfe.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://llj.cdnleiting.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xoi.mhx1999.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cpu.zdqjudy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bbo.haohaochexian.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bhk.xziqi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lel.mhx1999.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://nlh.quarkkingdee.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://itv.cdnleiting.top

[P04] 求长度
来源：http://wmz.haohaochexian.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://loe.aibaodan.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://srx.ywan-chungtsiang.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ubr.haohaochexian.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fid.gzhubu.top

Java: list.size();  map.size();  s.length()
来源：http://bjr.yueranfly.top

Go:   len(arr);  len(m)
来源：http://lfx.xingfuxueyuan.xyz

Ruby: x.length;  x.size
来源：http://wmc.hnxiangtu.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://wdp.yvedp.cn

[P05] 判断两个对象内容是否相等
来源：http://ezm.sysykeji.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://qod.sjlbkw.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lyb.yj20258888.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wux.sufxvd.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://obx.ydjk.org.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rle.wangshuangyany.cn

Go:   reflect.DeepEqual(a, b)
来源：http://zzb.zhijiandao.cn

Ruby: a == b
来源：http://nce.bjfxy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zle.0kj1m.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xib.zhiwuduotai.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://cdw.uphjek.com

PHP:  if (empty($x)) {}
来源：http://mfi.meibo888.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fgj.shanyushiyangtech.top

TS:   if (x == null) {}
来源：http://ieg.fzhhl.top

Java: if (x == null || x.isEmpty()) {}
来源：http://jwt.bjfxy.top

Go:   if x == nil {}
来源：http://mbr.ppjwa.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vfy.haohaochexian.top

C#:   if (x is null) {}
来源：http://plt.jyoumei.cn

[P07] 防抖与节流
来源：http://elx.hysaishi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lel.nanxuanxn.top

PHP:  // 手写时间戳比较
来源：http://aab.kuanghao11.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iqb.cucudq.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vhe.xuanzx.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ijz.ywan-chungtsiang.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ncs.smart0.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://bmp.zhijiandao.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jqt.zhoulong.xyz

[P08] 处理浮点精度问题
来源：http://yqg.ywan-chungtsiang.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mau.tian-w.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://snu.0kj1m.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lif.ybcxt.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://raz.pycfn.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ljt.bbcook.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fng.wangshuangyany.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://btz.xuanzx.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pjs.hysaishi.cn

================================================================================
来源：http://gjy.chenlongwang.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://htp.chenzaomai.com

================================================================================
来源：http://ywa.fzhhl.top

[Q01] 创建表
来源：http://qbp.yfazqb.com

CREATE TABLE users (
来源：http://rrt.ydzc1.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ceh.zdqjudy.top

name VARCHAR(50) NOT NULL,
来源：http://unf.c1oappe.top

email VARCHAR(100) UNIQUE,
来源：http://sfo.ybcxt.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://foh.gaohongyu789.top

);
来源：http://llm.yonumen.top

[Q02] 创建带外键的表
来源：http://hor.fzhhl.top

CREATE TABLE orders (
来源：http://olt.dashuyun.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jxy.52xcode.cn

user_id INT NOT NULL,
来源：http://yuq.jqgfzy.top

amount DECIMAL(10, 2),
来源：http://bde.cashguo.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dow.pycfn.com

);
来源：http://zib.tian-w.cn

[Q03] 增加列
来源：http://wnv.wangdashe.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xgm.hysaishi.cn

[Q04] 修改列类型
来源：http://auy.hnxiangtu.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dhu.havefunace.top

[Q05] 重命名列
来源：http://cbt.shanyushiyangkeji.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kky.xziqi.cn

[Q06] 删除列
来源：http://hrh.sweek.top

ALTER TABLE users DROP COLUMN age;
来源：http://vbs.andypj.xyz

[Q07] 删除表
来源：http://ule.9152youxi.cn

DROP TABLE IF EXISTS orders;
来源：http://pjw.gaohongyu789.top

[Q08] 创建普通索引
来源：http://tpg.xingfuxueyuan.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://tqw.daxiang520.top

[Q09] 创建唯一索引
来源：http://qeb.jinqigfzy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qyt.jqgufenzy.top

[Q10] 插入单行
来源：http://upt.chenlongwang.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://cmt.aizwys.cn

[Q11] 一次插入多行
来源：http://ist.yuanzhike.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://tqo.jianghu66.top

[Q12] 插入后取自增 ID
来源：http://vdi.yuanzhike.top

INSERT INTO users (name) VALUES ('C');
来源：http://don.cdnleiting.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jkj.xuanzx.com

[Q13] 忽略重复插入
来源：http://whq.c1oappe.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ndi.nanxinkj.top

[Q14] 存在则更新（upsert）
来源：http://lta.zycfv.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://htx.yj20258.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://muf.jqgfzy.top

[Q15] 查询全部
来源：http://wkz.sysykeji.top

SELECT * FROM users;
来源：http://frl.yvedp.cn

[Q16] 查询指定列
来源：http://uwp.nwbrower.top

SELECT id, name FROM users;
来源：http://sfs.0kj1m.cn

[Q17] 条件查询
来源：http://qkw.jinyuanbaomall.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://eqd.jinghuilouyu.cn

[Q18] 模糊匹配
来源：http://owq.ehwqpu.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wuk.aizwys.cn

[Q19] 范围查询
来源：http://nrz.cheryme.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ole.ehwqpu.com

[Q20] IN 列表
来源：http://jzn.tanke756.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qyj.zycfv.cn

[Q21] 空值判断
来源：http://xmb.yanxiufei.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://jwc.smart0.xyz

[Q22] 排序
来源：http://kiq.wangdashe.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rvb.pengpengdd.cyou

[Q23] 分页
来源：http://tqj.jinqigufen.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tlz.nwbrower.top

[Q24] 去重
来源：http://pzg.ppjwa.cn

SELECT DISTINCT city FROM users;
来源：http://zzx.hcnkem.com

[Q25] 只取前 N 条
来源：http://vfz.birdmap.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zfq.ywan-chungtsiang.top

[Q26] 计数
来源：http://ofx.jinyuanbaomall.cn

SELECT COUNT(*) FROM users;
来源：http://oya.jlsjyb.cn

[Q27] 条件计数
来源：http://vie.fanxiaobao.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://iba.xuetiantiany.cn

[Q28] 求和与平均
来源：http://sxi.shuidangran.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rkm.gaohongyu789.top

[Q29] 最大最小值
来源：http://xox.yj20258888.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://cyd.quarkkingdee.top

[Q30] 分组统计
来源：http://yun.sysykeji.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hma.gotoacloud.top

[Q31] 分组后过滤
来源：http://our.9152youxi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mfj.yj20258888.top

[Q32] 分组拼接字符串
来源：http://rox.guowangkeji.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mbm.jinghuilouyu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mal.xuanzx.com

[Q33] 多列分组
来源：http://kcm.yuxming.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fzz.guannengcc.top

[Q34] 每组取第一条
来源：http://vyn.uphjek.com

SELECT * FROM (
来源：http://wow.yongpay.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dbh.tianlin.xyz

) t WHERE rn = 1;
来源：http://suf.ydzc1.top

[Q35] 内连接
来源：http://yvm.shzxlz.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jwd.xingfuxueyuan.xyz

[Q36] 左连接
来源：http://ckp.cdnleiting.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kfd.yanxiufei.cn

[Q37] 右连接
来源：http://trv.epnwcf.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pva.sxryk.cn

[Q38] 全外连接（PostgreSQL）
来源：http://fzb.jinyuanbaomall.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yir.tanke756.top

[Q39] 自连接（查上下级）
来源：http://len.smart0.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://nqp.ivvv.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://eip.jyoumei.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://aes.jinqigufen.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://yeb.tarul.cn

[Q41] 多表连接
来源：http://yxo.hnqzz.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://emn.xinyue.icu

JOIN users u ON u.id = o.user_id
来源：http://hcw.hongshengwenyu.top

JOIN products p ON p.id = o.product_id;
来源：http://bgo.xuanzx.com

[Q42] 连接条件附加过滤
来源：http://ftm.tianlin.xyz

SELECT u.name, o.amount FROM users u
来源：http://osk.mhx1999.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ayd.0kj1m.cn

[Q43] 标量子查询
来源：http://opp.snrcjt.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qts.xuanzx.com

[Q44] IN 子查询
来源：http://bkq.pengpengdd.cyou

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://cjo.cdnleiting.top

[Q45] EXISTS 判断存在
来源：http://hno.xylfe.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://oom.zhaomingkeji.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://stl.zycfv.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yzc.yanxiufei.cn

[Q47] 与平均值比较
来源：http://vce.hnxiangtu.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xlb.hywenlv.cn

[Q48] CTE 公用表表达式
来源：http://xyd.jlsjyb.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zzp.aizwys.cn

SELECT * FROM t WHERE c > 5;
来源：http://kaa.jianghu66.top

[Q49] 更新单行
来源：http://jll.zhaomingkeji.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gcl.xinyue.icu

[Q50] 批量更新
来源：http://qcx.hnqzz.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fow.52xcode.cn

[Q51] 用子查询更新
来源：http://wir.hywenlv.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://kfy.tian-w.cn

[Q52] 删除指定行
来源：http://ash.316326.xyz

DELETE FROM users WHERE id = 10;
来源：http://vwg.yuxming.cn

[Q53] 按条件删除
来源：http://iho.uphjek.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yyh.jyoumei.cn

[Q54] 清空表
来源：http://ugu.yangfankeji.com

TRUNCATE TABLE logs;
来源：http://iqa.yangfankeji.com

[Q55] 排名（并列占位）
来源：http://wmu.jinghuilouyu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mto.shanyushiyangkeji.top

[Q56] 密集排名（并列不占位）
来源：http://ggy.fengsongda.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xnp.xuetiantiany.cn

[Q57] 行号
来源：http://zfb.gzhubu.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jka.fzhhl.top

[Q58] 累计求和
来源：http://yas.fanxiaobao.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xqc.jlsjyb.cn

[Q59] 分组内累计
来源：http://pvf.dianchejie.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://egz.ivvv.top

[Q60] 取上一行 / 下一行
来源：http://pux.xinyue.icu

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ufg.nwbrower.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ynh.jyoumei.cn

[Q61] 移动平均
来源：http://mze.zycfv.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ygr.jlsjyb.cn

[Q62] 分组占比
来源：http://haw.hnqzz.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pfc.zhongyouzk.top

[Q63] 开启事务
来源：http://fdq.gotoacloud.top

START TRANSACTION;                -- 或 BEGIN
来源：http://jxt.jinyuanbaomall.cn

[Q64] 提交事务
来源：http://fvw.xziqi.cn

COMMIT;
来源：http://vuq.nanxuanxn.top

[Q65] 回滚事务
来源：http://url.sxryk.cn

ROLLBACK;
来源：http://iyd.feifeiyinyue.top

[Q66] 行锁查询
来源：http://ppc.yueranfly.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xdy.daria6918.cn

[Q67] 设置隔离级别
来源：http://sqb.cheryme.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ebe.cucudq.cn

[Q68] 保存点
来源：http://xgd.pengpengdd.cyou

SAVEPOINT sp1;
来源：http://tob.havefunace.top

ROLLBACK TO sp1;
来源：http://xgo.gogol.net.cn

[Q69] 查看执行计划
来源：http://lev.jinqigfzy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nzo.sufxvd.cn

[Q70] 更新统计信息
来源：http://gqz.hfpthk.cn

ANALYZE TABLE users;
来源：http://twj.jinghuilouyu.cn

[Q71] 查看建表语句
来源：http://ejs.nanxinkj.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qrg.chenlongwang.top

[Q72] 查看索引
来源：http://tvp.jinyuanbaomall.cn

SHOW INDEX FROM users;
来源：http://wgt.wangshuangyany.cn

[Q73] 查看表状态
来源：http://wqh.xinyue.icu

SHOW TABLE STATUS LIKE 'users';
来源：http://wxt.zdqjudy.top

[Q74] 强制使用索引
来源：http://ynw.xinyue.icu

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jwy.gotoacloud.top

[Q75] 日期格式化
来源：http://ywm.sweek.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://nhx.zhiwuduotai.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rzl.yj202588.top


<!-- 参考信息 -->
代发 wailian999

TS:   // worker_threads 线程池
来源：http://xha.aizwys.cn

Java: Executors.newFixedThreadPool(4)
来源：http://wya.pengpengdd.cyou

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ypj.zhiwuduotai.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lsi.nwbrower.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ksu.xingfuxueyuan.xyz

[O03] 加锁保护共享数据
来源：http://vfv.jinqigufen.top

Py:   with lock: shared += 1
来源：http://ldv.dashuyun.cn

PHP:  // 用 flock() 做文件锁
来源：http://ruz.ppjwa.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cnf.tarul.cn

TS:   // 同 JS
来源：http://bfg.nwbrower.top

Java: synchronized (this) { shared++; }
来源：http://nah.zhengqikj.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qsm.cucudq.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://vzx.shangyingyoupin.top

C#:   lock (gate) { shared++; }
来源：http://zrn.tarul.cn

[O04] 定义异步函数并等待
来源：http://fdy.daria6918.cn

Py:   async def f():⏎    await g()
来源：http://wtl.sysykeji.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gjq.jinqigufen.top

JS:   async function f() { await g(); }
来源：http://qgw.hnqzz.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://gst.jinyuanbaomall.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ruc.pycfn.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ups.dianchejie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://owm.hesvh.cn

C#:   async Task F() { await G(); }
来源：http://lzk.yj202588.top

[O05] 并发执行并等待全部完成
来源：http://kes.cucudq.cn

Py:   asyncio.gather(*tasks)
来源：http://odc.nanxuanxn.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lgr.yongpay.top

JS:   await Promise.all(tasks)
来源：http://ukm.yuanzhike.top

TS:   await Promise.all(tasks)
来源：http://zvl.pycfn.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fmr.yfazqb.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qqv.hammf.cn

Ruby: threads.map(&:join)
来源：http://bdd.cucudq.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://scz.yuanzhike.top

[O06] 使用进程池
来源：http://rlu.shuidangran.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vau.feifeiyinyue.top

PHP:  // pcntl_fork 或多进程队列
来源：http://dxc.zycfv.cn

JS:   // child_process / cluster 模块
来源：http://fzr.mhx1999.top

TS:   // child_process / cluster 模块
来源：http://hho.zhoulong.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dbu.ywan-chungtsiang.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://acm.ywan-chungtsiang.top

Ruby: // fork 块
来源：http://bgf.gaohongyu789.top

C#:   Parallel.For
来源：http://vsi.zhixingplan.top

================================================================================
来源：http://lfc.xuetiantiany.cn

P. 常用工具函数
来源：http://utn.gotoacloud.top

================================================================================
来源：http://jwi.yangfankeji.com

[P01] 生成 UUID
来源：http://ato.dashuyun.cn

Py:   str(uuid.uuid4())
来源：http://etq.dianchejie.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zzz.redwolf501.top

JS:   crypto.randomUUID()
来源：http://tkz.havefunace.top

TS:   crypto.randomUUID()
来源：http://ngl.hfpthk.cn

Java: UUID.randomUUID().toString()
来源：http://fnt.fanxiaobao.xyz

Go:   // 用 github.com/google/uuid
来源：http://cyi.yuxming.cn

Ruby: SecureRandom.uuid
来源：http://rqx.gotoacloud.top

C#:   Guid.NewGuid().ToString()
来源：http://grp.hywenlv.cn

[P02] MD5 / SHA256 摘要
来源：http://afr.bjfxy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lin.yj20258.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://qsg.jinghuilouyu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ybw.ydjk.org.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mye.birdmap.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vgm.hysaishi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hux.zhoulong.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hxp.feifeiyinyue.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dyf.ydjk.org.cn

[P03] 生成短随机字符串
来源：http://hae.jqgfzy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xih.pengpengdd.cyou

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xrz.zhixingplan.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jno.zhijiandao.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mvg.zhoulong.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://awu.yueranfly.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yaq.bjfxy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ihr.ybcxt.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://eiu.aibaodan.cn

[P04] 求长度
来源：http://rzz.daxiang520.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uzn.cucudq.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rly.bjfxy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xuw.yvedp.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://abp.tanke756.top

Java: list.size();  map.size();  s.length()
来源：http://vma.yj202588.top

Go:   len(arr);  len(m)
来源：http://zve.vqdsnc.cn

Ruby: x.length;  x.size
来源：http://poa.zhoulong.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://jii.pengpengdd.cyou

[P05] 判断两个对象内容是否相等
来源：http://gaz.kuanghao11.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://wvp.ctjpmb.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pfv.tianlin.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://uji.cucudq.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fsp.zdbjq.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jek.bjfxy.top

Go:   reflect.DeepEqual(a, b)
来源：http://jfr.nwbrower.top

Ruby: a == b
来源：http://enr.ehwqpu.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nho.guowangkeji.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rul.xuetiantiany.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://myo.gogol.net.cn

PHP:  if (empty($x)) {}
来源：http://wpi.aibaodan.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pxs.ivvv.top

TS:   if (x == null) {}
来源：http://xhv.yueranfly.top

Java: if (x == null || x.isEmpty()) {}
来源：http://kvx.ydjk.org.cn

Go:   if x == nil {}
来源：http://ksi.birdmap.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pbr.aibaodan.cn

C#:   if (x is null) {}
来源：http://zpj.fktsv.cn

[P07] 防抖与节流
来源：http://wso.jianghu66.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zfv.chenlongwang.top

PHP:  // 手写时间戳比较
来源：http://ywi.sjlbkw.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mod.xuetiantiany.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jqw.sweek.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pfi.tian-w.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://uup.svipenyu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://een.hnxiangtu.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nqs.hywenlv.cn

[P08] 处理浮点精度问题
来源：http://zah.haohaochexian.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://psh.zycfv.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bxc.xylfe.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vbd.zhengqikj.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nho.cqqwz.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wxk.tarul.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zqa.jianghu66.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zfb.guowangkeji.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pze.andypj.xyz

================================================================================
来源：http://qtw.aibaodan.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ttw.jianghu66.top

================================================================================
来源：http://rxm.jinqigufen.top

[Q01] 创建表
来源：http://gyd.jqgfzy.top

CREATE TABLE users (
来源：http://wes.gaohongyu789.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tsf.ybcxt.top

name VARCHAR(50) NOT NULL,
来源：http://oty.hongshengwenyu.top

email VARCHAR(100) UNIQUE,
来源：http://adn.yj20258888.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://crr.kuanghao11.cn

);
来源：http://kye.zhijiandao.cn

[Q02] 创建带外键的表
来源：http://djr.hnqzz.top

CREATE TABLE orders (
来源：http://vud.shanyushiyangkeji.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://byw.smart0.xyz

user_id INT NOT NULL,
来源：http://gyl.guowangkeji.top

amount DECIMAL(10, 2),
来源：http://yqq.snrcjt.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://poa.quarkkingdee.top

);
来源：http://ult.gzhubu.top

[Q03] 增加列
来源：http://bmf.zhongyouzk.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://map.daxiang520.top

[Q04] 修改列类型
来源：http://gsc.smart0.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mgm.wangdashe.top

[Q05] 重命名列
来源：http://vcr.hfpthk.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xyo.zhongyouzk.top

[Q06] 删除列
来源：http://knq.nanxuanxn.top

ALTER TABLE users DROP COLUMN age;
来源：http://duy.xziqi.cn

[Q07] 删除表
来源：http://bsr.wangshuangyany.cn

DROP TABLE IF EXISTS orders;
来源：http://mcg.pycfn.com

[Q08] 创建普通索引
来源：http://hqx.meibo888.top

CREATE INDEX idx_users_email ON users(email);
来源：http://bpi.jinqigufen.top

[Q09] 创建唯一索引
来源：http://vfp.birdmap.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fpr.iojbl.cn

[Q10] 插入单行
来源：http://pez.jinqigufen.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dzg.bjfxy.top

[Q11] 一次插入多行
来源：http://bjx.ydjk.org.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://swu.sufxvd.cn

[Q12] 插入后取自增 ID
来源：http://iad.dianchejie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://axy.wangshuangyany.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qmn.c1oappe.top

[Q13] 忽略重复插入
来源：http://uyu.hcnkem.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nax.zhijiandao.cn

[Q14] 存在则更新（upsert）
来源：http://jdl.sjlbkw.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://sfx.yongpay.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mwa.fzhhl.top

[Q15] 查询全部
来源：http://agq.xinyue.icu

SELECT * FROM users;
来源：http://hgw.hongshengwenyu.top

[Q16] 查询指定列
来源：http://fcw.tian-w.cn

SELECT id, name FROM users;
来源：http://xxu.ivvv.top

[Q17] 条件查询
来源：http://mbz.zdbjq.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cwp.jyoumei.cn

[Q18] 模糊匹配
来源：http://mwb.cashguo.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kqt.ydjk.org.cn

[Q19] 范围查询
来源：http://yrl.xingfuxueyuan.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qbg.sufxvd.cn

[Q20] IN 列表
来源：http://zzn.hywenlv.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://puf.yj202588.top

[Q21] 空值判断
来源：http://uld.yj202588.top

SELECT * FROM users WHERE email IS NULL;
来源：http://iae.wangshuangyany.cn

[Q22] 排序
来源：http://tru.pycfn.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jhf.guannengcc.top

[Q23] 分页
来源：http://pfk.hesvh.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://sni.zhengqikj.top

[Q24] 去重
来源：http://iaw.fzhhl.top

SELECT DISTINCT city FROM users;
来源：http://kts.yj20258888.top

[Q25] 只取前 N 条
来源：http://icw.sufxvd.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hbn.gotoacloud.top

[Q26] 计数
来源：http://llt.aizwys.cn

SELECT COUNT(*) FROM users;
来源：http://efm.yj202588.top

[Q27] 条件计数
来源：http://dah.sweek.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jvu.yueranfly.top

[Q28] 求和与平均
来源：http://uev.xuanzx.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://exj.ydjk.org.cn

[Q29] 最大最小值
来源：http://cxd.vqdsnc.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://htj.vqdsnc.cn

[Q30] 分组统计
来源：http://ifu.yueranfly.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zrl.fehbvm.com

[Q31] 分组后过滤
来源：http://rav.tian-w.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vjb.zhijiandao.cn

[Q32] 分组拼接字符串
来源：http://lqb.guowangkeji.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pep.hammf.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ufi.pengpengdd.cyou

[Q33] 多列分组
来源：http://ejy.tanke756.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://sbf.zhiwuduotai.top

[Q34] 每组取第一条
来源：http://mcl.ppjwa.cn

SELECT * FROM (
来源：http://nor.cdnleiting.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fit.daria6918.cn

) t WHERE rn = 1;
来源：http://lgu.chenlongwang.top

[Q35] 内连接
来源：http://xcn.svipenyu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rlx.zhiwuduotai.top

[Q36] 左连接
来源：http://rrs.nanxinkj.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bwn.fzhhl.top

[Q37] 右连接
来源：http://qgl.yj202588.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ezz.tianlin.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://tuj.zhoulong.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://thd.xinyue.icu

[Q39] 自连接（查上下级）
来源：http://tog.tian-w.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://rzh.pycfn.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mjp.yvedp.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://qpq.quarkkingdee.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rcv.pycfn.com

[Q41] 多表连接
来源：http://vet.cashguo.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://tpv.hesvh.cn

JOIN users u ON u.id = o.user_id
来源：http://zss.zdbjq.cn

JOIN products p ON p.id = o.product_id;
来源：http://vjo.cheryme.top

[Q42] 连接条件附加过滤
来源：http://yor.tanke756.top

SELECT u.name, o.amount FROM users u
来源：http://rny.jyoumei.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hhu.yfazqb.com

[Q43] 标量子查询
来源：http://bhr.shzxlz.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kew.meibo888.top

[Q44] IN 子查询
来源：http://qkx.sufxvd.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://glz.gogol.net.cn

[Q45] EXISTS 判断存在
来源：http://gyz.shangyingyoupin.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yro.dashuyun.cn

[Q46] NOT EXISTS 判断不存在
来源：http://uzu.yuxming.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jik.cdnleiting.top

[Q47] 与平均值比较
来源：http://mno.hysaishi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tlq.c1oappe.top

[Q48] CTE 公用表表达式
来源：http://ahm.jiagoushi.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ehwqpu.com

SELECT * FROM t WHERE c > 5;
来源：http://yfy.ybcxt.top

[Q49] 更新单行
来源：http://cbf.ehwqpu.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://erl.cdnleiting.top

[Q50] 批量更新
来源：http://kqi.cucudq.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://sys.ehwqpu.com

[Q51] 用子查询更新
来源：http://vxh.chenjidiqi.icu

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lol.jqgfzy.top

[Q52] 删除指定行
来源：http://mxe.jyoumei.cn

DELETE FROM users WHERE id = 10;
来源：http://mev.yanxiufei.cn

[Q53] 按条件删除
来源：http://osl.dianchejie.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://klp.yj20258888.top

[Q54] 清空表
来源：http://sri.xuanzx.com

TRUNCATE TABLE logs;
来源：http://suo.jinqigufen.top

[Q55] 排名（并列占位）
来源：http://yqe.hcnkem.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hvg.gzhubu.top

[Q56] 密集排名（并列不占位）
来源：http://ilc.ctjpmb.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rqp.yanxiufei.cn

[Q57] 行号
来源：http://ytb.zhongyouzk.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mkr.daria6918.cn

[Q58] 累计求和
来源：http://psm.yj20258.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wuf.cqqwz.cn

[Q59] 分组内累计
来源：http://zsy.yj202588.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://udb.yvedp.cn

[Q60] 取上一行 / 下一行
来源：http://zsy.hesvh.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ine.cashguo.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wpj.hnqzz.top

[Q61] 移动平均
来源：http://xyw.epnwcf.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ihr.yonumen.top

[Q62] 分组占比
来源：http://zsq.mhx1999.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://iai.jinqigufen.top

[Q63] 开启事务
来源：http://gtq.tianlin.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://zwg.fanxiaobao.xyz

[Q64] 提交事务
来源：http://cnf.chenjidiqi.icu

COMMIT;
来源：http://kcu.dashuyun.cn

[Q65] 回滚事务
来源：http://ufe.xinyue.icu

ROLLBACK;
来源：http://kkl.cucudq.cn

[Q66] 行锁查询
来源：http://tpu.nwbrower.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wki.aibaodan.cn

[Q67] 设置隔离级别
来源：http://gra.redwolf501.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ccy.yvedp.cn

[Q68] 保存点
来源：http://axy.vehdjk.com

SAVEPOINT sp1;
来源：http://qhu.daria6918.cn

ROLLBACK TO sp1;
来源：http://wxt.ybcxt.top

[Q69] 查看执行计划
来源：http://eyn.ctjpmb.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://eqw.nanxuanxn.top

[Q70] 更新统计信息
来源：http://qve.hesvh.cn

ANALYZE TABLE users;
来源：http://xzp.ivvv.top

[Q71] 查看建表语句
来源：http://nfr.chenjidiqi.icu

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mjd.wangdashe.top

[Q72] 查看索引
来源：http://fvs.tarul.cn

SHOW INDEX FROM users;
来源：http://wpz.hongshengwenyu.top

[Q73] 查看表状态
来源：http://buu.hfpthk.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://guj.tian-w.cn

[Q74] 强制使用索引
来源：http://xiu.xziqi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mjp.jqgufenzy.top

[Q75] 日期格式化
来源：http://kvk.smart0.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tqd.yj202588.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://izt.ywan-chungtsiang.top

[Q76] 按天统计
来源：http://qej.svipenyu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vmt.aizwys.cn

[Q77] 时间加减
来源：http://iae.ppjwa.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vzn.nanxinkj.top

[Q78] 当前时间
来源：http://sdm.tarul.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jht.pycfn.com

[Q79] 字符串拼接
来源：http://vuo.zdqjudy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://umx.tian-w.cn


<!-- 参考信息 -->
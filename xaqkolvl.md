代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kqc.havefunace.top

[O03] 加锁保护共享数据
来源：http://gqw.chenzaomai.com

Py:   with lock: shared += 1
来源：http://csg.zhoulong.xyz

PHP:  // 用 flock() 做文件锁
来源：http://tyk.yj202588.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ias.yongpay.top

TS:   // 同 JS
来源：http://zqo.havefunace.top

Java: synchronized (this) { shared++; }
来源：http://dfl.hysaishi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ayk.jianghu66.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://qjt.jianghu66.top

C#:   lock (gate) { shared++; }
来源：http://fvf.yangfankeji.com

[O04] 定义异步函数并等待
来源：http://hzj.haohaochexian.top

Py:   async def f():⏎    await g()
来源：http://sjo.zdbjq.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kyh.zhoulong.xyz

JS:   async function f() { await g(); }
来源：http://rrf.yangfankeji.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://pxj.yj202588.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cvu.hysaishi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://uwq.yongpay.top

Ruby: # 用 Fiber 或 async gem
来源：http://nqq.epnwcf.com

C#:   async Task F() { await G(); }
来源：http://lep.aizwys.cn

[O05] 并发执行并等待全部完成
来源：http://dbx.yanxiufei.cn

Py:   asyncio.gather(*tasks)
来源：http://vip.chenjidiqi.icu

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lua.pengpengdd.cyou

JS:   await Promise.all(tasks)
来源：http://teo.smart0.xyz

TS:   await Promise.all(tasks)
来源：http://sfa.ydzc1.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gkv.jiagoushi.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qvs.yonumen.top

Ruby: threads.map(&:join)
来源：http://wli.chenzaomai.com

C#:   await Task.WhenAll(t1, t2)
来源：http://oui.shzxlz.cn

[O06] 使用进程池
来源：http://vei.zhijiandao.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xmm.xingfuxueyuan.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://scf.birdmap.top

JS:   // child_process / cluster 模块
来源：http://oyu.yanxiufei.cn

TS:   // child_process / cluster 模块
来源：http://mpj.wangdashe.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lub.zhiwuduotai.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wxg.c1oappe.top

Ruby: // fork 块
来源：http://czk.sysykeji.top

C#:   Parallel.For
来源：http://cow.aizwys.cn

================================================================================
来源：http://nkj.fzhhl.top

P. 常用工具函数
来源：http://ndp.fktsv.cn

================================================================================
来源：http://zij.wangshuangyany.cn

[P01] 生成 UUID
来源：http://afk.gogol.net.cn

Py:   str(uuid.uuid4())
来源：http://drr.hnqzz.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kpk.vqdsnc.cn

JS:   crypto.randomUUID()
来源：http://fxl.ydjk.org.cn

TS:   crypto.randomUUID()
来源：http://qgw.wangdashe.top

Java: UUID.randomUUID().toString()
来源：http://hji.birdmap.top

Go:   // 用 github.com/google/uuid
来源：http://umr.andypj.xyz

Ruby: SecureRandom.uuid
来源：http://bpf.xingfuxueyuan.xyz

C#:   Guid.NewGuid().ToString()
来源：http://thy.shuidangran.top

[P02] MD5 / SHA256 摘要
来源：http://hpn.epnwcf.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vga.nanxuanxn.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://kdd.zhijiandao.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ivy.uphjek.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jfd.zhijiandao.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mvi.ybcxt.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hsy.cheryme.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://auo.tarul.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://buc.316326.xyz

[P03] 生成短随机字符串
来源：http://jqw.tarul.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ene.xingfuxueyuan.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cvh.fktsv.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nqh.fengsongda.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yho.ybcxt.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zxj.aibaodan.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fwj.316326.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://zmp.chenzaomai.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kwi.shangyingyoupin.top

[P04] 求长度
来源：http://ayn.hywenlv.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qlz.gogol.net.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uit.sysykeji.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://szc.vehdjk.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ike.ctjpmb.com

Java: list.size();  map.size();  s.length()
来源：http://jvk.snrcjt.cn

Go:   len(arr);  len(m)
来源：http://ydo.birdmap.top

Ruby: x.length;  x.size
来源：http://nyi.shanyushiyangtech.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ihn.wangdashe.top

[P05] 判断两个对象内容是否相等
来源：http://dnr.yuanzhike.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://mnp.chenjidiqi.icu

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kal.sufxvd.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://auf.vehdjk.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fkb.hnqzz.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://teg.shanyushiyangkeji.top

Go:   reflect.DeepEqual(a, b)
来源：http://qai.pycfn.com

Ruby: a == b
来源：http://zrk.guannengcc.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hff.jyoumei.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mje.epnwcf.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fec.pengpengdd.cyou

PHP:  if (empty($x)) {}
来源：http://ewv.yonumen.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mxo.andypj.xyz

TS:   if (x == null) {}
来源：http://yxm.cashguo.top

Java: if (x == null || x.isEmpty()) {}
来源：http://pgy.shzxlz.cn

Go:   if x == nil {}
来源：http://qhg.feifeiyinyue.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lfl.dashuyun.cn

C#:   if (x is null) {}
来源：http://diy.daria6918.cn

[P07] 防抖与节流
来源：http://toq.meibo888.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://scl.snrcjt.cn

PHP:  // 手写时间戳比较
来源：http://ywt.zhengqikj.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kkk.daxiang520.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pyy.yvedp.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gsy.hammf.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kqk.jinqigufen.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://cum.chenlongwang.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://oat.cqqwz.cn

[P08] 处理浮点精度问题
来源：http://viu.9152youxi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://itt.gotoacloud.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wce.hnxiangtu.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mqn.zycfv.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lfj.yueranfly.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ngf.tanke756.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ipn.xziqi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hxn.nwbrower.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ugx.snrcjt.cn

================================================================================
来源：http://zhk.jianghu66.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yai.hnxiangtu.top

================================================================================
来源：http://zdu.ppjwa.cn

[Q01] 创建表
来源：http://ykg.chenjidiqi.icu

CREATE TABLE users (
来源：http://utx.dianchejie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wkg.wangdashe.top

name VARCHAR(50) NOT NULL,
来源：http://nat.epnwcf.com

email VARCHAR(100) UNIQUE,
来源：http://tbe.fzhhl.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://omp.jinghuilouyu.cn

);
来源：http://iei.zycfv.cn

[Q02] 创建带外键的表
来源：http://sqy.sufxvd.cn

CREATE TABLE orders (
来源：http://waj.c1oappe.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ijc.zhoulong.xyz

user_id INT NOT NULL,
来源：http://sgk.yuanzhike.top

amount DECIMAL(10, 2),
来源：http://bgt.0kj1m.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dlg.gogol.net.cn

);
来源：http://wfz.iojbl.cn

[Q03] 增加列
来源：http://bir.quarkkingdee.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nrz.smart0.xyz

[Q04] 修改列类型
来源：http://msw.tarul.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://htf.gzhubu.top

[Q05] 重命名列
来源：http://wxg.ydjk.org.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://phr.jinqigufen.top

[Q06] 删除列
来源：http://ryb.yueranfly.top

ALTER TABLE users DROP COLUMN age;
来源：http://hgi.hesvh.cn

[Q07] 删除表
来源：http://mee.zycfv.cn

DROP TABLE IF EXISTS orders;
来源：http://kes.jqgufenzy.top

[Q08] 创建普通索引
来源：http://uui.sysykeji.top

CREATE INDEX idx_users_email ON users(email);
来源：http://yiu.gaohongyu789.top

[Q09] 创建唯一索引
来源：http://oew.birdmap.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tid.fehbvm.com

[Q10] 插入单行
来源：http://omc.sxryk.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pgv.dashuyun.cn

[Q11] 一次插入多行
来源：http://zem.pycfn.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hnh.yangfankeji.com

[Q12] 插入后取自增 ID
来源：http://auu.jyoumei.cn

INSERT INTO users (name) VALUES ('C');
来源：http://icq.nanxuanxn.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zsk.yvedp.cn

[Q13] 忽略重复插入
来源：http://onw.shuidangran.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ppf.fengsongda.top

[Q14] 存在则更新（upsert）
来源：http://viy.sufxvd.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dwq.guowangkeji.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fgp.hnxiangtu.top

[Q15] 查询全部
来源：http://fdn.havefunace.top

SELECT * FROM users;
来源：http://uur.nanxinkj.top

[Q16] 查询指定列
来源：http://kqp.sxryk.cn

SELECT id, name FROM users;
来源：http://csn.ivvv.top

[Q17] 条件查询
来源：http://oel.xylfe.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://emw.gogol.net.cn

[Q18] 模糊匹配
来源：http://ihq.chenzaomai.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://oys.shanyushiyangkeji.top

[Q19] 范围查询
来源：http://fmd.tanke756.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ful.hfpthk.cn

[Q20] IN 列表
来源：http://zms.gaohongyu789.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yym.jinghuilouyu.cn

[Q21] 空值判断
来源：http://hxb.bjfxy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://htj.fktsv.cn

[Q22] 排序
来源：http://gfu.hongshengwenyu.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hdb.tian-w.cn

[Q23] 分页
来源：http://brv.nwbrower.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zdc.gotoacloud.top

[Q24] 去重
来源：http://rhf.yuanzhike.top

SELECT DISTINCT city FROM users;
来源：http://znk.chenzaomai.com

[Q25] 只取前 N 条
来源：http://rma.xuanzx.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://aka.ctjpmb.com

[Q26] 计数
来源：http://ank.zhengqikj.top

SELECT COUNT(*) FROM users;
来源：http://cmb.jqgufenzy.top

[Q27] 条件计数
来源：http://sut.haohaochexian.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jxg.dashuyun.cn

[Q28] 求和与平均
来源：http://lcr.zdqjudy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tsd.daria6918.cn

[Q29] 最大最小值
来源：http://abo.zhongyouzk.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://jkd.sysykeji.top

[Q30] 分组统计
来源：http://xgy.ydjk.org.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jnu.hongshengwenyu.top

[Q31] 分组后过滤
来源：http://ztj.uphjek.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://obg.tarul.cn

[Q32] 分组拼接字符串
来源：http://nay.tanke756.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xmm.yvedp.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://scu.daxiang520.top

[Q33] 多列分组
来源：http://jse.tanke756.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://yri.iojbl.cn

[Q34] 每组取第一条
来源：http://kbo.yfazqb.com

SELECT * FROM (
来源：http://oso.vehdjk.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://oln.0kj1m.cn

) t WHERE rn = 1;
来源：http://sgp.svipenyu.cn

[Q35] 内连接
来源：http://fdl.fzhhl.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://nsb.wangshuangyany.cn

[Q36] 左连接
来源：http://csa.vehdjk.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mob.yongpay.top

[Q37] 右连接
来源：http://azx.ivvv.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ier.ydzc1.top

[Q38] 全外连接（PostgreSQL）
来源：http://zdv.yfazqb.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bdy.yj20258.top

[Q39] 自连接（查上下级）
来源：http://jzz.jiagoushi.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://hqe.zycfv.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://orb.guowangkeji.top

[Q40] 交叉连接（笛卡尔积）
来源：http://xdz.9152youxi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://eus.cucudq.cn

[Q41] 多表连接
来源：http://wvo.yj202588.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://jhq.cheryme.top

JOIN users u ON u.id = o.user_id
来源：http://ski.jinyuanbaomall.cn

JOIN products p ON p.id = o.product_id;
来源：http://cil.daria6918.cn

[Q42] 连接条件附加过滤
来源：http://lfc.yj20258.top

SELECT u.name, o.amount FROM users u
来源：http://bub.hongshengwenyu.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jaa.yfazqb.com

[Q43] 标量子查询
来源：http://mpi.9152youxi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bgp.hywenlv.cn

[Q44] IN 子查询
来源：http://chp.mhx1999.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xby.guowangkeji.top

[Q45] EXISTS 判断存在
来源：http://ies.bjfxy.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hvh.smart0.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://oyj.fktsv.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ncb.nanxinkj.top

[Q47] 与平均值比较
来源：http://occ.cucudq.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://eoi.shzxlz.cn

[Q48] CTE 公用表表达式
来源：http://owp.sxryk.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ihg.uphjek.com

SELECT * FROM t WHERE c > 5;
来源：http://yvz.hcnkem.com

[Q49] 更新单行
来源：http://jjd.andypj.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pbv.quarkkingdee.top

[Q50] 批量更新
来源：http://qwm.meibo888.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://noo.zhiwuduotai.top

[Q51] 用子查询更新
来源：http://bdj.xylfe.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vku.hammf.cn

[Q52] 删除指定行
来源：http://eqs.jinqigfzy.top

DELETE FROM users WHERE id = 10;
来源：http://bxc.hywenlv.cn

[Q53] 按条件删除
来源：http://rbs.shanyushiyangtech.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qhu.ivvv.top

[Q54] 清空表
来源：http://kyl.xuetiantiany.cn

TRUNCATE TABLE logs;
来源：http://ywa.nanxinkj.top

[Q55] 排名（并列占位）
来源：http://xrf.guannengcc.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://oid.andypj.xyz

[Q56] 密集排名（并列不占位）
来源：http://dle.vqdsnc.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vzn.sjlbkw.cn

[Q57] 行号
来源：http://peh.tarul.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://him.gotoacloud.top

[Q58] 累计求和
来源：http://xwd.quarkkingdee.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kzo.sjlbkw.cn

[Q59] 分组内累计
来源：http://fgs.yangfankeji.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ctm.yongpay.top

[Q60] 取上一行 / 下一行
来源：http://jdu.jyoumei.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://iyf.nwbrower.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dnp.yangfankeji.com

[Q61] 移动平均
来源：http://ouq.xziqi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ijh.yvedp.cn

[Q62] 分组占比
来源：http://nyt.zhengqikj.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://yvg.pycfn.com

[Q63] 开启事务
来源：http://wgi.c1oappe.top

START TRANSACTION;                -- 或 BEGIN
来源：http://vos.0kj1m.cn

[Q64] 提交事务
来源：http://wgr.svipenyu.cn

COMMIT;
来源：http://gwu.hongshengwenyu.top

[Q65] 回滚事务
来源：http://roq.aizwys.cn

ROLLBACK;
来源：http://vmh.9152youxi.cn

[Q66] 行锁查询
来源：http://quk.andypj.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://aho.fktsv.cn

[Q67] 设置隔离级别
来源：http://feg.jqgfzy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://viv.zhixingplan.top

[Q68] 保存点
来源：http://wny.cqqwz.cn

SAVEPOINT sp1;
来源：http://ekl.zhengqikj.top

ROLLBACK TO sp1;
来源：http://ygf.epnwcf.com

[Q69] 查看执行计划
来源：http://vav.zdqjudy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zzm.hfpthk.cn

[Q70] 更新统计信息
来源：http://xep.ppjwa.cn

ANALYZE TABLE users;
来源：http://muj.sjlbkw.cn

[Q71] 查看建表语句
来源：http://iws.yangfankeji.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cbu.fktsv.cn

[Q72] 查看索引
来源：http://cqd.zhoulong.xyz

SHOW INDEX FROM users;
来源：http://rue.yuanzhike.top

[Q73] 查看表状态
来源：http://kws.fktsv.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://qgo.guowangkeji.top

[Q74] 强制使用索引
来源：http://wxk.jinqigfzy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zbv.yangfankeji.com

[Q75] 日期格式化
来源：http://znr.pycfn.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dxw.zycfv.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://srx.jinqigufen.top

[Q76] 按天统计
来源：http://nhj.sufxvd.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tgy.yj20258.top

[Q77] 时间加减
来源：http://wer.yuanzhike.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://plp.xziqi.cn

[Q78] 当前时间
来源：http://rbu.cqqwz.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://sba.fzhhl.top

[Q79] 字符串拼接
来源：http://eji.chenjidiqi.icu

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cur.snrcjt.cn

[Q80] 字符串截取
来源：http://pau.zhengqikj.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ejs.zhixingplan.top

[Q81] 字符串替换
来源：http://mjx.zhongyouzk.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mds.jlsjyb.cn


<!-- 参考信息 -->
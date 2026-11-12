代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pvy.ydjk.org.cn

TS:   // 同 JS
来源：http://zuc.guannengcc.top

Java: synchronized (this) { shared++; }
来源：http://ryu.hywenlv.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bqf.bjfxy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://kdi.iojbl.cn

C#:   lock (gate) { shared++; }
来源：http://buc.sysykeji.top

[O04] 定义异步函数并等待
来源：http://vzh.yj202588.top

Py:   async def f():⏎    await g()
来源：http://qve.epnwcf.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hid.iojbl.cn

JS:   async function f() { await g(); }
来源：http://lfc.yangfankeji.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://anf.fktsv.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://aol.bjfxy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tfx.jqgfzy.top

Ruby: # 用 Fiber 或 async gem
来源：http://owh.redwolf501.top

C#:   async Task F() { await G(); }
来源：http://jqh.zhengqikj.top

[O05] 并发执行并等待全部完成
来源：http://yfr.xziqi.cn

Py:   asyncio.gather(*tasks)
来源：http://gsr.fehbvm.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zek.fzhhl.top

JS:   await Promise.all(tasks)
来源：http://ofp.0kj1m.cn

TS:   await Promise.all(tasks)
来源：http://ibn.yj202588.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://aoq.hnqzz.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tpx.zhengqikj.top

Ruby: threads.map(&:join)
来源：http://fob.jinqigfzy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://chy.9152youxi.cn

[O06] 使用进程池
来源：http://uem.hysaishi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pov.aizwys.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://tlp.chenzaomai.com

JS:   // child_process / cluster 模块
来源：http://bor.zdqjudy.top

TS:   // child_process / cluster 模块
来源：http://zzn.fehbvm.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://nge.hcnkem.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ljq.guannengcc.top

Ruby: // fork 块
来源：http://bkd.jlsjyb.cn

C#:   Parallel.For
来源：http://slt.redwolf501.top

================================================================================
来源：http://mpt.feifeiyinyue.top

P. 常用工具函数
来源：http://iim.fanxiaobao.xyz

================================================================================
来源：http://thv.zhijiandao.cn

[P01] 生成 UUID
来源：http://tcv.hongshengwenyu.top

Py:   str(uuid.uuid4())
来源：http://ufq.ctjpmb.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://oni.guowangkeji.top

JS:   crypto.randomUUID()
来源：http://uso.hesvh.cn

TS:   crypto.randomUUID()
来源：http://ayt.gotoacloud.top

Java: UUID.randomUUID().toString()
来源：http://ren.shanyushiyangtech.top

Go:   // 用 github.com/google/uuid
来源：http://raj.zhengqikj.top

Ruby: SecureRandom.uuid
来源：http://lzh.kuanghao11.cn

C#:   Guid.NewGuid().ToString()
来源：http://xlh.dianchejie.cn

[P02] MD5 / SHA256 摘要
来源：http://ryj.jiagoushi.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://uey.sxryk.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hki.shuidangran.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vac.chenzaomai.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wmo.hongshengwenyu.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kpr.aizwys.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cls.shanyushiyangtech.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hlq.iojbl.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sjj.hnqzz.top

[P03] 生成短随机字符串
来源：http://uey.xuetiantiany.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qvj.jqgfzy.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zze.fengsongda.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gyz.zhengqikj.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vim.gaohongyu789.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jyl.aibaodan.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://upj.hesvh.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ohq.ppjwa.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rpx.jyoumei.cn

[P04] 求长度
来源：http://gli.nwbrower.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://snc.ydzc1.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qeq.gogol.net.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jtt.haohaochexian.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ilf.sysykeji.top

Java: list.size();  map.size();  s.length()
来源：http://mec.xinyue.icu

Go:   len(arr);  len(m)
来源：http://kok.jyoumei.cn

Ruby: x.length;  x.size
来源：http://sxy.hesvh.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://lew.gaohongyu789.top

[P05] 判断两个对象内容是否相等
来源：http://sgt.c1oappe.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://nzj.cucudq.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rob.haohaochexian.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wda.cqqwz.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://frb.feifeiyinyue.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zuv.aizwys.cn

Go:   reflect.DeepEqual(a, b)
来源：http://hxk.sufxvd.cn

Ruby: a == b
来源：http://pat.feifeiyinyue.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cbv.iojbl.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://liu.yangfankeji.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://cic.wangshuangyany.cn

PHP:  if (empty($x)) {}
来源：http://lyr.tarul.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ukl.hnxiangtu.top

TS:   if (x == null) {}
来源：http://qhf.9152youxi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://bet.gotoacloud.top

Go:   if x == nil {}
来源：http://hkj.zdbjq.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://prd.daxiang520.top

C#:   if (x is null) {}
来源：http://feq.hnqzz.top

[P07] 防抖与节流
来源：http://zhs.ctjpmb.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://yed.meibo888.top

PHP:  // 手写时间戳比较
来源：http://mkz.xylfe.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://drw.hnqzz.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nfe.andypj.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qkq.ctjpmb.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://elo.c1oappe.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://lkp.tarul.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ixz.chenzaomai.com

[P08] 处理浮点精度问题
来源：http://joe.zhixingplan.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wxx.iojbl.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://aun.fktsv.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://erb.yueranfly.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tzf.jinyuanbaomall.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vlo.shuidangran.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rgy.zdqjudy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zgr.daria6918.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://srh.tian-w.cn

================================================================================
来源：http://zwx.birdmap.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kdd.chenzaomai.com

================================================================================
来源：http://zjk.fengsongda.top

[Q01] 创建表
来源：http://zxy.guannengcc.top

CREATE TABLE users (
来源：http://fps.dashuyun.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vfz.yfazqb.com

name VARCHAR(50) NOT NULL,
来源：http://xso.hesvh.cn

email VARCHAR(100) UNIQUE,
来源：http://dui.fehbvm.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://dvj.hesvh.cn

);
来源：http://gvt.zdqjudy.top

[Q02] 创建带外键的表
来源：http://bye.fehbvm.com

CREATE TABLE orders (
来源：http://ffy.pycfn.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ina.shanyushiyangkeji.top

user_id INT NOT NULL,
来源：http://cfk.zdqjudy.top

amount DECIMAL(10, 2),
来源：http://kkc.yanxiufei.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zyl.sxryk.cn

);
来源：http://uqs.316326.xyz

[Q03] 增加列
来源：http://siw.dianchejie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://top.wangshuangyany.cn

[Q04] 修改列类型
来源：http://lzj.316326.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://sro.uphjek.com

[Q05] 重命名列
来源：http://kma.hesvh.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dgl.yj20258.top

[Q06] 删除列
来源：http://rht.52xcode.cn

ALTER TABLE users DROP COLUMN age;
来源：http://snf.zhongyouzk.top

[Q07] 删除表
来源：http://kfb.cheryme.top

DROP TABLE IF EXISTS orders;
来源：http://fnt.xuanzx.com

[Q08] 创建普通索引
来源：http://uyq.xziqi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ery.shanyushiyangtech.top

[Q09] 创建唯一索引
来源：http://rsu.tarul.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xfv.fehbvm.com

[Q10] 插入单行
来源：http://mus.vqdsnc.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tzu.iojbl.cn

[Q11] 一次插入多行
来源：http://ffv.cucudq.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://end.jinqigufen.top

[Q12] 插入后取自增 ID
来源：http://kvu.sjlbkw.cn

INSERT INTO users (name) VALUES ('C');
来源：http://cad.fengsongda.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gzs.fengsongda.top

[Q13] 忽略重复插入
来源：http://fjy.wangshuangyany.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gvx.jinghuilouyu.cn

[Q14] 存在则更新（upsert）
来源：http://dte.kuanghao11.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rth.bjfxy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://syq.tian-w.cn

[Q15] 查询全部
来源：http://vzi.jqgufenzy.top

SELECT * FROM users;
来源：http://exn.pycfn.com

[Q16] 查询指定列
来源：http://ueb.sjlbkw.cn

SELECT id, name FROM users;
来源：http://stk.ehwqpu.com

[Q17] 条件查询
来源：http://xbf.dashuyun.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://adw.yj202588.top

[Q18] 模糊匹配
来源：http://hpe.guowangkeji.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://fss.zhaomingkeji.xyz

[Q19] 范围查询
来源：http://kjr.jinqigfzy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://eze.jianghu66.top

[Q20] IN 列表
来源：http://jsg.gzhubu.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wbj.nanxinkj.top

[Q21] 空值判断
来源：http://kbw.ydjk.org.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://uho.zhijiandao.cn

[Q22] 排序
来源：http://yph.jinqigfzy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dlo.yuxming.cn

[Q23] 分页
来源：http://uwt.hnxiangtu.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gwr.fzhhl.top

[Q24] 去重
来源：http://zrv.fktsv.cn

SELECT DISTINCT city FROM users;
来源：http://lzx.havefunace.top

[Q25] 只取前 N 条
来源：http://pnv.hnqzz.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nlq.9152youxi.cn

[Q26] 计数
来源：http://jat.zhiwuduotai.top

SELECT COUNT(*) FROM users;
来源：http://otg.yonumen.top

[Q27] 条件计数
来源：http://urb.316326.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hic.fengsongda.top

[Q28] 求和与平均
来源：http://ruo.wangdashe.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kds.ydjk.org.cn

[Q29] 最大最小值
来源：http://qvu.yongpay.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://awo.zhaomingkeji.xyz

[Q30] 分组统计
来源：http://lrw.zdbjq.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wte.ppjwa.cn

[Q31] 分组后过滤
来源：http://rmf.yangfankeji.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mci.xuanzx.com

[Q32] 分组拼接字符串
来源：http://xxr.daxiang520.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fzw.dashuyun.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qvd.jinghuilouyu.cn

[Q33] 多列分组
来源：http://jcu.c1oappe.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qvz.pengpengdd.cyou

[Q34] 每组取第一条
来源：http://ngu.iojbl.cn

SELECT * FROM (
来源：http://cgj.zhaomingkeji.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://uxa.jyoumei.cn

) t WHERE rn = 1;
来源：http://exv.yangfankeji.com

[Q35] 内连接
来源：http://ppx.uphjek.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://dni.xinyue.icu

[Q36] 左连接
来源：http://spu.tian-w.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vqy.pycfn.com

[Q37] 右连接
来源：http://gtz.fehbvm.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vpe.xuetiantiany.cn

[Q38] 全外连接（PostgreSQL）
来源：http://bxj.cheryme.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dxk.kuanghao11.cn

[Q39] 自连接（查上下级）
来源：http://gvb.ehwqpu.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://zwi.zycfv.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rrz.bjfxy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://hxc.kuanghao11.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qyq.hywenlv.cn

[Q41] 多表连接
来源：http://uxb.fehbvm.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://uyq.fanxiaobao.xyz

JOIN users u ON u.id = o.user_id
来源：http://wbx.jyoumei.cn

JOIN products p ON p.id = o.product_id;
来源：http://mxv.zhengqikj.top

[Q42] 连接条件附加过滤
来源：http://res.yfazqb.com

SELECT u.name, o.amount FROM users u
来源：http://lwe.yfazqb.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gev.yanxiufei.cn

[Q43] 标量子查询
来源：http://oau.hysaishi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rrg.ybcxt.top

[Q44] IN 子查询
来源：http://jka.kuanghao11.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://epq.yuxming.cn

[Q45] EXISTS 判断存在
来源：http://frd.daria6918.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gtk.yonumen.top

[Q46] NOT EXISTS 判断不存在
来源：http://rqy.mhx1999.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mwb.zycfv.cn

[Q47] 与平均值比较
来源：http://tjc.havefunace.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bmu.jianghu66.top

[Q48] CTE 公用表表达式
来源：http://vbs.jlsjyb.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cmq.yongpay.top

SELECT * FROM t WHERE c > 5;
来源：http://ijh.xylfe.cn

[Q49] 更新单行
来源：http://kah.gogol.net.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lbb.birdmap.top

[Q50] 批量更新
来源：http://kvv.yonumen.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fkn.quarkkingdee.top

[Q51] 用子查询更新
来源：http://ocj.zhixingplan.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lxn.tianlin.xyz

[Q52] 删除指定行
来源：http://ddv.mhx1999.top

DELETE FROM users WHERE id = 10;
来源：http://ohl.xinyue.icu

[Q53] 按条件删除
来源：http://npq.ydzc1.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ide.hnxiangtu.top

[Q54] 清空表
来源：http://mdq.ivvv.top

TRUNCATE TABLE logs;
来源：http://rit.chenlongwang.top

[Q55] 排名（并列占位）
来源：http://cbn.jlsjyb.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jqj.ehwqpu.com

[Q56] 密集排名（并列不占位）
来源：http://hmc.dashuyun.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wgg.chenjidiqi.icu

[Q57] 行号
来源：http://cpb.hnqzz.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zgm.hfpthk.cn

[Q58] 累计求和
来源：http://xvv.fzhhl.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ksc.yj202588.top

[Q59] 分组内累计
来源：http://btk.jinghuilouyu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tmh.quarkkingdee.top

[Q60] 取上一行 / 下一行
来源：http://bpe.cashguo.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nor.epnwcf.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ifo.smart0.xyz

[Q61] 移动平均
来源：http://ioa.guowangkeji.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://abk.yj20258888.top

[Q62] 分组占比
来源：http://tsu.tianlin.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wef.zhijiandao.cn

[Q63] 开启事务
来源：http://zwz.cucudq.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://gky.haohaochexian.top

[Q64] 提交事务
来源：http://meu.tian-w.cn

COMMIT;
来源：http://mhj.nanxinkj.top

[Q65] 回滚事务
来源：http://jdj.xinyue.icu

ROLLBACK;
来源：http://ntg.sxryk.cn

[Q66] 行锁查询
来源：http://ifv.hnxiangtu.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pxp.sjlbkw.cn

[Q67] 设置隔离级别
来源：http://mww.jqgufenzy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cwl.shzxlz.cn

[Q68] 保存点
来源：http://vqe.quarkkingdee.top

SAVEPOINT sp1;
来源：http://bfp.haohaochexian.top

ROLLBACK TO sp1;
来源：http://rwr.hnqzz.top

[Q69] 查看执行计划
来源：http://vzj.pycfn.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rkw.aizwys.cn

[Q70] 更新统计信息
来源：http://ywl.zhengqikj.top

ANALYZE TABLE users;
来源：http://nlo.zdqjudy.top

[Q71] 查看建表语句
来源：http://lrh.hfpthk.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://csb.yvedp.cn

[Q72] 查看索引
来源：http://tjd.hywenlv.cn

SHOW INDEX FROM users;
来源：http://lad.andypj.xyz

[Q73] 查看表状态
来源：http://gxz.jinghuilouyu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://qbh.ydjk.org.cn

[Q74] 强制使用索引
来源：http://qxb.jinqigfzy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://nog.pycfn.com

[Q75] 日期格式化
来源：http://jvd.chenzaomai.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wow.cashguo.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://aaq.0kj1m.cn

[Q76] 按天统计
来源：http://est.havefunace.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dvn.gogol.net.cn

[Q77] 时间加减
来源：http://nii.shanyushiyangtech.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://aki.hammf.cn

[Q78] 当前时间
来源：http://cdz.gotoacloud.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fro.pycfn.com

[Q79] 字符串拼接
来源：http://kvr.bbcook.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cuj.yj20258.top

[Q80] 字符串截取
来源：http://atc.chenzaomai.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bri.ivvv.top

[Q81] 字符串替换
来源：http://anl.zdqjudy.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ztl.tanke756.top

[Q82] 字符长度与字节长度
来源：http://evw.gzhubu.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zes.gogol.net.cn

[Q83] 大小写转换
来源：http://xmr.yueranfly.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fkh.havefunace.top


<!-- 参考信息 -->
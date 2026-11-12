代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://tql.sjlbkw.cn

C#:   lock (gate) { shared++; }
来源：http://cxw.yangfankeji.com

[O04] 定义异步函数并等待
来源：http://zhf.hammf.cn

Py:   async def f():⏎    await g()
来源：http://sug.0kj1m.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zlm.tarul.cn

JS:   async function f() { await g(); }
来源：http://grq.fzhhl.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://zab.yj20258888.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mjw.sysykeji.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ywj.zhengqikj.top

Ruby: # 用 Fiber 或 async gem
来源：http://nce.shzxlz.cn

C#:   async Task F() { await G(); }
来源：http://tiq.wangshuangyany.cn

[O05] 并发执行并等待全部完成
来源：http://yoa.yuanzhike.top

Py:   asyncio.gather(*tasks)
来源：http://lxj.yangfankeji.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jcd.zycfv.cn

JS:   await Promise.all(tasks)
来源：http://oya.yueranfly.top

TS:   await Promise.all(tasks)
来源：http://dxg.zhaomingkeji.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qzo.zhaomingkeji.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vzm.uphjek.com

Ruby: threads.map(&:join)
来源：http://erj.ywan-chungtsiang.top

C#:   await Task.WhenAll(t1, t2)
来源：http://hvl.pengpengdd.cyou

[O06] 使用进程池
来源：http://bii.ctjpmb.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mnt.c1oappe.top

PHP:  // pcntl_fork 或多进程队列
来源：http://cfs.yfazqb.com

JS:   // child_process / cluster 模块
来源：http://zpf.xingfuxueyuan.xyz

TS:   // child_process / cluster 模块
来源：http://tcy.zhengqikj.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://loy.haohaochexian.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hgg.ehwqpu.com

Ruby: // fork 块
来源：http://jjc.bbcook.cn

C#:   Parallel.For
来源：http://fvv.shzxlz.cn

================================================================================
来源：http://zrp.gzhubu.top

P. 常用工具函数
来源：http://sft.xuetiantiany.cn

================================================================================
来源：http://yje.yangfankeji.com

[P01] 生成 UUID
来源：http://qdp.xinyue.icu

Py:   str(uuid.uuid4())
来源：http://omp.bjfxy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rwz.andypj.xyz

JS:   crypto.randomUUID()
来源：http://aej.aizwys.cn

TS:   crypto.randomUUID()
来源：http://lhm.yuxming.cn

Java: UUID.randomUUID().toString()
来源：http://ayi.jyoumei.cn

Go:   // 用 github.com/google/uuid
来源：http://tcn.wangshuangyany.cn

Ruby: SecureRandom.uuid
来源：http://ugk.jinqigfzy.top

C#:   Guid.NewGuid().ToString()
来源：http://kgn.hysaishi.cn

[P02] MD5 / SHA256 摘要
来源：http://vyh.ydzc1.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ooe.wangshuangyany.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hvw.ydjk.org.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pgb.yj202588.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://caj.wangdashe.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://exr.zhijiandao.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yjt.jyoumei.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://uil.havefunace.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://grh.yuxming.cn

[P03] 生成短随机字符串
来源：http://bra.shzxlz.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pir.jinghuilouyu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ajg.yuanzhike.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ucf.uphjek.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yta.tanke756.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qin.zdbjq.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bxp.ivvv.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://eii.hammf.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mru.shanyushiyangkeji.top

[P04] 求长度
来源：http://dzz.fehbvm.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vni.9152youxi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nmd.xylfe.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ngy.jinghuilouyu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tht.dashuyun.cn

Java: list.size();  map.size();  s.length()
来源：http://zja.yonumen.top

Go:   len(arr);  len(m)
来源：http://qbe.xuanzx.com

Ruby: x.length;  x.size
来源：http://cng.wangshuangyany.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ukq.gaohongyu789.top

[P05] 判断两个对象内容是否相等
来源：http://xas.xinyue.icu

Py:   a == b              # 列表与字典递归比较内容
来源：http://uoc.andypj.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xoy.hnqzz.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://csw.fengsongda.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jrc.zhijiandao.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kyk.fzhhl.top

Go:   reflect.DeepEqual(a, b)
来源：http://kkv.yj20258888.top

Ruby: a == b
来源：http://let.yfazqb.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://sgp.svipenyu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ung.guannengcc.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://alm.hesvh.cn

PHP:  if (empty($x)) {}
来源：http://giz.bjfxy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lnr.yanxiufei.cn

TS:   if (x == null) {}
来源：http://rog.jinyuanbaomall.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://oib.zhixingplan.top

Go:   if x == nil {}
来源：http://nuf.mhx1999.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rdn.hcnkem.com

C#:   if (x is null) {}
来源：http://ynn.bbcook.cn

[P07] 防抖与节流
来源：http://jtm.iojbl.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pps.haohaochexian.top

PHP:  // 手写时间戳比较
来源：http://ekp.hesvh.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zux.haohaochexian.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vsb.pycfn.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://axs.nwbrower.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rxu.zhiwuduotai.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://xcy.guannengcc.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kyv.zhoulong.xyz

[P08] 处理浮点精度问题
来源：http://qlo.zhaomingkeji.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lun.chenzaomai.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://owf.dashuyun.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gtr.gaohongyu789.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ysx.tanke756.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vtt.ywan-chungtsiang.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qoo.zhiwuduotai.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://nez.redwolf501.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mhy.jqgfzy.top

================================================================================
来源：http://wap.gzhubu.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dkv.hnxiangtu.top

================================================================================
来源：http://wbr.c1oappe.top

[Q01] 创建表
来源：http://qjl.fehbvm.com

CREATE TABLE users (
来源：http://kto.pengpengdd.cyou

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hji.yangfankeji.com

name VARCHAR(50) NOT NULL,
来源：http://tns.birdmap.top

email VARCHAR(100) UNIQUE,
来源：http://fec.fehbvm.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lzt.andypj.xyz

);
来源：http://fhk.xziqi.cn

[Q02] 创建带外键的表
来源：http://bho.yj20258.top

CREATE TABLE orders (
来源：http://ibd.ydjk.org.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xpc.feifeiyinyue.top

user_id INT NOT NULL,
来源：http://rlt.wangdashe.top

amount DECIMAL(10, 2),
来源：http://gqm.yuxming.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fde.fehbvm.com

);
来源：http://oxg.zhongyouzk.top

[Q03] 增加列
来源：http://pzm.fktsv.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tih.feifeiyinyue.top

[Q04] 修改列类型
来源：http://clu.tianlin.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mjw.andypj.xyz

[Q05] 重命名列
来源：http://yiw.zhoulong.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jlp.tanke756.top

[Q06] 删除列
来源：http://qrr.yj20258.top

ALTER TABLE users DROP COLUMN age;
来源：http://tns.mhx1999.top

[Q07] 删除表
来源：http://jas.shuidangran.top

DROP TABLE IF EXISTS orders;
来源：http://kbl.wangshuangyany.cn

[Q08] 创建普通索引
来源：http://nim.sjlbkw.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xlc.zhaomingkeji.xyz

[Q09] 创建唯一索引
来源：http://bvz.yj20258888.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zvr.dianchejie.cn

[Q10] 插入单行
来源：http://dhe.hysaishi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://sla.zhijiandao.cn

[Q11] 一次插入多行
来源：http://ujq.havefunace.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://shs.ivvv.top

[Q12] 插入后取自增 ID
来源：http://abr.bbcook.cn

INSERT INTO users (name) VALUES ('C');
来源：http://phc.hcnkem.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lvb.yongpay.top

[Q13] 忽略重复插入
来源：http://unh.ydzc1.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dav.fengsongda.top

[Q14] 存在则更新（upsert）
来源：http://hjb.ydjk.org.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wgx.sufxvd.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ukj.shzxlz.cn

[Q15] 查询全部
来源：http://mad.pycfn.com

SELECT * FROM users;
来源：http://lrc.sufxvd.cn

[Q16] 查询指定列
来源：http://ffz.haohaochexian.top

SELECT id, name FROM users;
来源：http://xzo.daria6918.cn

[Q17] 条件查询
来源：http://ceu.shanyushiyangtech.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qui.jqgufenzy.top

[Q18] 模糊匹配
来源：http://xam.daxiang520.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vmc.ydzc1.top

[Q19] 范围查询
来源：http://ayi.0kj1m.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://din.zhijiandao.cn

[Q20] IN 列表
来源：http://tuo.daria6918.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yub.havefunace.top

[Q21] 空值判断
来源：http://dzz.yangfankeji.com

SELECT * FROM users WHERE email IS NULL;
来源：http://bld.tian-w.cn

[Q22] 排序
来源：http://oiu.hywenlv.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ojz.gotoacloud.top

[Q23] 分页
来源：http://xwt.chenzaomai.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dzm.yuanzhike.top

[Q24] 去重
来源：http://sca.haohaochexian.top

SELECT DISTINCT city FROM users;
来源：http://kua.ivvv.top

[Q25] 只取前 N 条
来源：http://wue.ydzc1.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vpa.aizwys.cn

[Q26] 计数
来源：http://jul.pycfn.com

SELECT COUNT(*) FROM users;
来源：http://dqd.hongshengwenyu.top

[Q27] 条件计数
来源：http://asd.havefunace.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qmo.hfpthk.cn

[Q28] 求和与平均
来源：http://ffj.tian-w.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xvz.epnwcf.com

[Q29] 最大最小值
来源：http://mly.wangshuangyany.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://vmp.sysykeji.top

[Q30] 分组统计
来源：http://ayo.zhengqikj.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ozh.jinyuanbaomall.cn

[Q31] 分组后过滤
来源：http://tkq.zhixingplan.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kki.fktsv.cn

[Q32] 分组拼接字符串
来源：http://rqm.sjlbkw.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://syr.iojbl.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bth.jlsjyb.cn

[Q33] 多列分组
来源：http://yff.hesvh.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hzh.tian-w.cn

[Q34] 每组取第一条
来源：http://dyp.cdnleiting.top

SELECT * FROM (
来源：http://plo.wangdashe.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fdm.yonumen.top

) t WHERE rn = 1;
来源：http://wfp.hammf.cn

[Q35] 内连接
来源：http://zlx.sxryk.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://swe.ybcxt.top

[Q36] 左连接
来源：http://gof.shzxlz.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xik.jiagoushi.top

[Q37] 右连接
来源：http://nys.jinqigufen.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tsy.chenjidiqi.icu

[Q38] 全外连接（PostgreSQL）
来源：http://kqc.hnxiangtu.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mal.jiagoushi.top

[Q39] 自连接（查上下级）
来源：http://kaz.dashuyun.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://nzz.nanxinkj.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pcm.redwolf501.top

[Q40] 交叉连接（笛卡尔积）
来源：http://mvl.cdnleiting.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lny.guowangkeji.top

[Q41] 多表连接
来源：http://ohc.yueranfly.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ynz.fengsongda.top

JOIN users u ON u.id = o.user_id
来源：http://xdd.feifeiyinyue.top

JOIN products p ON p.id = o.product_id;
来源：http://ryl.yj20258.top

[Q42] 连接条件附加过滤
来源：http://skr.yuanzhike.top

SELECT u.name, o.amount FROM users u
来源：http://xnc.snrcjt.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wvr.redwolf501.top

[Q43] 标量子查询
来源：http://dcz.snrcjt.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hpn.gogol.net.cn

[Q44] IN 子查询
来源：http://idr.hcnkem.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jyk.tarul.cn

[Q45] EXISTS 判断存在
来源：http://whp.andypj.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rhy.jinghuilouyu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ttn.gzhubu.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bpb.feifeiyinyue.top

[Q47] 与平均值比较
来源：http://big.gzhubu.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tvk.52xcode.cn

[Q48] CTE 公用表表达式
来源：http://plg.zhongyouzk.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://flg.shangyingyoupin.top

SELECT * FROM t WHERE c > 5;
来源：http://yei.yangfankeji.com

[Q49] 更新单行
来源：http://atd.zhengqikj.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qlt.hcnkem.com

[Q50] 批量更新
来源：http://qbx.redwolf501.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hdc.zdbjq.cn

[Q51] 用子查询更新
来源：http://mvd.jinyuanbaomall.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qxd.cucudq.cn

[Q52] 删除指定行
来源：http://ugf.yj202588.top

DELETE FROM users WHERE id = 10;
来源：http://rza.hcnkem.com

[Q53] 按条件删除
来源：http://idi.svipenyu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://msd.redwolf501.top

[Q54] 清空表
来源：http://cwg.jinyuanbaomall.cn

TRUNCATE TABLE logs;
来源：http://ffx.wangdashe.top

[Q55] 排名（并列占位）
来源：http://faa.sjlbkw.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://etf.dianchejie.cn

[Q56] 密集排名（并列不占位）
来源：http://mak.xuanzx.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://eou.nanxinkj.top

[Q57] 行号
来源：http://cfy.gotoacloud.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://exe.yonumen.top

[Q58] 累计求和
来源：http://fhd.ivvv.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mso.zhixingplan.top

[Q59] 分组内累计
来源：http://dls.bjfxy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jzq.havefunace.top

[Q60] 取上一行 / 下一行
来源：http://kfa.smart0.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://aui.shanyushiyangkeji.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://luv.jiagoushi.top

[Q61] 移动平均
来源：http://yit.guowangkeji.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wre.jinghuilouyu.cn

[Q62] 分组占比
来源：http://luy.hongshengwenyu.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mov.yueranfly.top

[Q63] 开启事务
来源：http://hym.haohaochexian.top

START TRANSACTION;                -- 或 BEGIN
来源：http://miv.dianchejie.cn

[Q64] 提交事务
来源：http://hze.hesvh.cn

COMMIT;
来源：http://htq.0kj1m.cn

[Q65] 回滚事务
来源：http://wlb.yonumen.top

ROLLBACK;
来源：http://fdf.vqdsnc.cn

[Q66] 行锁查询
来源：http://wqq.bjfxy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vwp.guannengcc.top

[Q67] 设置隔离级别
来源：http://abd.zycfv.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wsd.yuanzhike.top

[Q68] 保存点
来源：http://flp.pycfn.com

SAVEPOINT sp1;
来源：http://ssl.yj202588.top

ROLLBACK TO sp1;
来源：http://udx.52xcode.cn

[Q69] 查看执行计划
来源：http://uyw.hysaishi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://uhp.shuidangran.top

[Q70] 更新统计信息
来源：http://omj.316326.xyz

ANALYZE TABLE users;
来源：http://jsy.yj20258.top

[Q71] 查看建表语句
来源：http://spe.pengpengdd.cyou

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://iel.mhx1999.top

[Q72] 查看索引
来源：http://cro.nanxuanxn.top

SHOW INDEX FROM users;
来源：http://qfy.zhongyouzk.top

[Q73] 查看表状态
来源：http://uxg.nanxinkj.top

SHOW TABLE STATUS LIKE 'users';
来源：http://pbt.fengsongda.top

[Q74] 强制使用索引
来源：http://qum.hfpthk.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ebs.zhongyouzk.top

[Q75] 日期格式化
来源：http://nfk.zdqjudy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lay.vehdjk.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wax.hcnkem.com

[Q76] 按天统计
来源：http://ayp.pengpengdd.cyou

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ebn.fengsongda.top

[Q77] 时间加减
来源：http://btf.cucudq.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wbf.cqqwz.cn

[Q78] 当前时间
来源：http://aiv.cdnleiting.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gdi.sjlbkw.cn

[Q79] 字符串拼接
来源：http://jho.yj20258.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uqj.aizwys.cn

[Q80] 字符串截取
来源：http://aqo.feifeiyinyue.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://uyh.ivvv.top

[Q81] 字符串替换
来源：http://jtu.epnwcf.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hrx.jinqigufen.top

[Q82] 字符长度与字节长度
来源：http://gds.fehbvm.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pvg.cucudq.cn

[Q83] 大小写转换
来源：http://iqi.hnxiangtu.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://onj.yuanzhike.top

[Q84] 去除首尾空格
来源：http://fsq.cashguo.top

SELECT TRIM(name) FROM users;
来源：http://nmf.aibaodan.cn

[Q85] 数值取整
来源：http://ppr.c1oappe.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hgt.haohaochexian.top


<!-- 参考信息 -->
代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://wxn.xinyue.icu

C#:   lock (gate) { shared++; }
来源：http://txe.9152youxi.cn

[O04] 定义异步函数并等待
来源：http://cxg.yfazqb.com

Py:   async def f():⏎    await g()
来源：http://ypu.xinyue.icu

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gom.ywan-chungtsiang.top

JS:   async function f() { await g(); }
来源：http://ewh.dianchejie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://xst.hywenlv.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://alf.hammf.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tzw.wangshuangyany.cn

Ruby: # 用 Fiber 或 async gem
来源：http://irj.hesvh.cn

C#:   async Task F() { await G(); }
来源：http://ilf.fengsongda.top

[O05] 并发执行并等待全部完成
来源：http://fbb.gaohongyu789.top

Py:   asyncio.gather(*tasks)
来源：http://qnd.xuetiantiany.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gpb.haohaochexian.top

JS:   await Promise.all(tasks)
来源：http://qje.cqqwz.cn

TS:   await Promise.all(tasks)
来源：http://lqz.yueranfly.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://nwz.gogol.net.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ueb.xuetiantiany.cn

Ruby: threads.map(&:join)
来源：http://zsh.yueranfly.top

C#:   await Task.WhenAll(t1, t2)
来源：http://pls.iojbl.cn

[O06] 使用进程池
来源：http://rzg.nanxuanxn.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tqa.hfpthk.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://gws.shzxlz.cn

JS:   // child_process / cluster 模块
来源：http://nte.ywan-chungtsiang.top

TS:   // child_process / cluster 模块
来源：http://vju.shanyushiyangtech.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://abl.sxryk.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://del.bjfxy.top

Ruby: // fork 块
来源：http://vis.ywan-chungtsiang.top

C#:   Parallel.For
来源：http://qsh.yanxiufei.cn

================================================================================
来源：http://jrz.sxryk.cn

P. 常用工具函数
来源：http://mee.dianchejie.cn

================================================================================
来源：http://wnn.mhx1999.top

[P01] 生成 UUID
来源：http://mql.aizwys.cn

Py:   str(uuid.uuid4())
来源：http://qpk.zdbjq.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rfk.sjlbkw.cn

JS:   crypto.randomUUID()
来源：http://uwg.ctjpmb.com

TS:   crypto.randomUUID()
来源：http://ied.gaohongyu789.top

Java: UUID.randomUUID().toString()
来源：http://utl.haohaochexian.top

Go:   // 用 github.com/google/uuid
来源：http://aot.hcnkem.com

Ruby: SecureRandom.uuid
来源：http://rgo.zdqjudy.top

C#:   Guid.NewGuid().ToString()
来源：http://jmj.hcnkem.com

[P02] MD5 / SHA256 摘要
来源：http://tqx.zhaomingkeji.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gva.jiagoushi.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://jdt.redwolf501.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ukd.nwbrower.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://frp.tarul.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ler.yonumen.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qky.nanxuanxn.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fmk.tian-w.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kjw.nanxinkj.top

[P03] 生成短随机字符串
来源：http://smy.tanke756.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nqe.zycfv.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://glg.jlsjyb.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dgt.cheryme.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lzq.jianghu66.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://znz.jinqigfzy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ztp.jiagoushi.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://rlt.tarul.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://sdx.zycfv.cn

[P04] 求长度
来源：http://lzw.yanxiufei.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ull.hcnkem.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://efu.ehwqpu.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://srn.ywan-chungtsiang.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sna.zhongyouzk.top

Java: list.size();  map.size();  s.length()
来源：http://zvc.yuxming.cn

Go:   len(arr);  len(m)
来源：http://avz.vqdsnc.cn

Ruby: x.length;  x.size
来源：http://cwz.xuanzx.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://tks.hnxiangtu.top

[P05] 判断两个对象内容是否相等
来源：http://qmw.hfpthk.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://pbe.dianchejie.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xhc.daria6918.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vfy.chenzaomai.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cvj.redwolf501.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ypx.ctjpmb.com

Go:   reflect.DeepEqual(a, b)
来源：http://azs.zhixingplan.top

Ruby: a == b
来源：http://tcd.guowangkeji.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://maf.jinyuanbaomall.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pdd.redwolf501.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jjo.yuxming.cn

PHP:  if (empty($x)) {}
来源：http://nyp.hongshengwenyu.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ebx.zhongyouzk.top

TS:   if (x == null) {}
来源：http://kbc.xylfe.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://pfv.zhijiandao.cn

Go:   if x == nil {}
来源：http://hks.bjfxy.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pwe.jinqigufen.top

C#:   if (x is null) {}
来源：http://hii.yj202588.top

[P07] 防抖与节流
来源：http://qjn.ctjpmb.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mbe.fzhhl.top

PHP:  // 手写时间戳比较
来源：http://zor.meibo888.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lux.meibo888.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gst.xinyue.icu

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zef.svipenyu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tza.aibaodan.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://vox.xuetiantiany.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nrk.epnwcf.com

[P08] 处理浮点精度问题
来源：http://oot.hammf.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://txy.jinyuanbaomall.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gah.xingfuxueyuan.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://axy.dianchejie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lrq.xingfuxueyuan.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mpx.fktsv.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fgf.tanke756.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://eap.zdbjq.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jba.xingfuxueyuan.xyz

================================================================================
来源：http://yve.tianlin.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lrr.fengsongda.top

================================================================================
来源：http://cdh.ivvv.top

[Q01] 创建表
来源：http://rvy.bjfxy.top

CREATE TABLE users (
来源：http://gfe.quarkkingdee.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vvs.jinghuilouyu.cn

name VARCHAR(50) NOT NULL,
来源：http://pwz.jyoumei.cn

email VARCHAR(100) UNIQUE,
来源：http://hnk.zhijiandao.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vvm.shzxlz.cn

);
来源：http://raw.vehdjk.com

[Q02] 创建带外键的表
来源：http://ufb.sjlbkw.cn

CREATE TABLE orders (
来源：http://yjv.gogol.net.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hpm.fktsv.cn

user_id INT NOT NULL,
来源：http://vqf.jinghuilouyu.cn

amount DECIMAL(10, 2),
来源：http://igj.daxiang520.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ubf.fanxiaobao.xyz

);
来源：http://rda.shuidangran.top

[Q03] 增加列
来源：http://irb.cqqwz.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://egp.fktsv.cn

[Q04] 修改列类型
来源：http://cne.fanxiaobao.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gxz.quarkkingdee.top

[Q05] 重命名列
来源：http://zwq.cqqwz.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lpn.xingfuxueyuan.xyz

[Q06] 删除列
来源：http://teh.chenlongwang.top

ALTER TABLE users DROP COLUMN age;
来源：http://ksi.epnwcf.com

[Q07] 删除表
来源：http://pal.hammf.cn

DROP TABLE IF EXISTS orders;
来源：http://fbw.sjlbkw.cn

[Q08] 创建普通索引
来源：http://ekv.shanyushiyangtech.top

CREATE INDEX idx_users_email ON users(email);
来源：http://asj.cucudq.cn

[Q09] 创建唯一索引
来源：http://yzd.sweek.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fqj.ydjk.org.cn

[Q10] 插入单行
来源：http://uhd.jyoumei.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dmn.iojbl.cn

[Q11] 一次插入多行
来源：http://mwl.yj20258.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://irh.jinqigufen.top

[Q12] 插入后取自增 ID
来源：http://fda.xuetiantiany.cn

INSERT INTO users (name) VALUES ('C');
来源：http://jxb.gzhubu.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ivy.jinqigufen.top

[Q13] 忽略重复插入
来源：http://ncz.aibaodan.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fla.pycfn.com

[Q14] 存在则更新（upsert）
来源：http://xzh.guannengcc.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ldi.hysaishi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gza.ctjpmb.com

[Q15] 查询全部
来源：http://cyu.zdqjudy.top

SELECT * FROM users;
来源：http://rfp.uphjek.com

[Q16] 查询指定列
来源：http://rwu.kuanghao11.cn

SELECT id, name FROM users;
来源：http://oot.c1oappe.top

[Q17] 条件查询
来源：http://yis.xuetiantiany.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lgs.ppjwa.cn

[Q18] 模糊匹配
来源：http://mkx.yj202588.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://uhx.mhx1999.top

[Q19] 范围查询
来源：http://uyf.smart0.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://njk.xinyue.icu

[Q20] IN 列表
来源：http://vno.wangshuangyany.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fzj.aibaodan.cn

[Q21] 空值判断
来源：http://mrl.jqgfzy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://nnn.uphjek.com

[Q22] 排序
来源：http://nku.ybcxt.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ohs.yfazqb.com

[Q23] 分页
来源：http://bzw.yj202588.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ybv.jiagoushi.top

[Q24] 去重
来源：http://dkf.jinghuilouyu.cn

SELECT DISTINCT city FROM users;
来源：http://hto.yuxming.cn

[Q25] 只取前 N 条
来源：http://hst.guannengcc.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://uio.ydjk.org.cn

[Q26] 计数
来源：http://hgf.zhongyouzk.top

SELECT COUNT(*) FROM users;
来源：http://jcr.cqqwz.cn

[Q27] 条件计数
来源：http://vim.birdmap.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zil.vqdsnc.cn

[Q28] 求和与平均
来源：http://ixl.smart0.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://riv.zhaomingkeji.xyz

[Q29] 最大最小值
来源：http://ftn.jinqigfzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://kgx.jinghuilouyu.cn

[Q30] 分组统计
来源：http://zyr.andypj.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ncz.cdnleiting.top

[Q31] 分组后过滤
来源：http://wra.jqgufenzy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://znl.hammf.cn

[Q32] 分组拼接字符串
来源：http://xio.vqdsnc.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dni.zdbjq.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hrm.epnwcf.com

[Q33] 多列分组
来源：http://xbx.snrcjt.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kfs.daxiang520.top

[Q34] 每组取第一条
来源：http://mrf.cashguo.top

SELECT * FROM (
来源：http://lvc.andypj.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ifn.sweek.top

) t WHERE rn = 1;
来源：http://svy.9152youxi.cn

[Q35] 内连接
来源：http://wxk.fehbvm.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mhc.epnwcf.com

[Q36] 左连接
来源：http://end.snrcjt.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fmc.zhongyouzk.top

[Q37] 右连接
来源：http://wuq.jianghu66.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://trz.wangdashe.top

[Q38] 全外连接（PostgreSQL）
来源：http://qxq.vehdjk.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ogp.dashuyun.cn

[Q39] 自连接（查上下级）
来源：http://frd.shangyingyoupin.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://uzg.sysykeji.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lan.hnxiangtu.top

[Q40] 交叉连接（笛卡尔积）
来源：http://lss.mhx1999.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hxg.hfpthk.cn

[Q41] 多表连接
来源：http://jji.gzhubu.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://qns.52xcode.cn

JOIN users u ON u.id = o.user_id
来源：http://orl.yfazqb.com

JOIN products p ON p.id = o.product_id;
来源：http://oen.ywan-chungtsiang.top

[Q42] 连接条件附加过滤
来源：http://bez.xinyue.icu

SELECT u.name, o.amount FROM users u
来源：http://vas.tarul.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://uis.ydzc1.top

[Q43] 标量子查询
来源：http://fzz.fanxiaobao.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qwo.fanxiaobao.xyz

[Q44] IN 子查询
来源：http://jvu.jinyuanbaomall.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://czu.haohaochexian.top

[Q45] EXISTS 判断存在
来源：http://zxl.epnwcf.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://epb.xuanzx.com

[Q46] NOT EXISTS 判断不存在
来源：http://lrg.cheryme.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mhs.aibaodan.cn

[Q47] 与平均值比较
来源：http://pnj.hnqzz.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mvf.bbcook.cn

[Q48] CTE 公用表表达式
来源：http://dco.fanxiaobao.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vvw.dianchejie.cn

SELECT * FROM t WHERE c > 5;
来源：http://jwo.yanxiufei.cn

[Q49] 更新单行
来源：http://lfu.gogol.net.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://sjg.zhoulong.xyz

[Q50] 批量更新
来源：http://xnr.yongpay.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vdw.hnxiangtu.top

[Q51] 用子查询更新
来源：http://cqp.yongpay.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zvm.shzxlz.cn

[Q52] 删除指定行
来源：http://xhn.meibo888.top

DELETE FROM users WHERE id = 10;
来源：http://xwg.sjlbkw.cn

[Q53] 按条件删除
来源：http://aim.jinqigfzy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://flf.yangfankeji.com

[Q54] 清空表
来源：http://svf.ydzc1.top

TRUNCATE TABLE logs;
来源：http://qei.zycfv.cn

[Q55] 排名（并列占位）
来源：http://peg.xinyue.icu

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://uum.pengpengdd.cyou

[Q56] 密集排名（并列不占位）
来源：http://ecj.zdqjudy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ugd.ydzc1.top

[Q57] 行号
来源：http://xme.shanyushiyangtech.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fnq.sjlbkw.cn

[Q58] 累计求和
来源：http://fzc.yj20258888.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jgx.vehdjk.com

[Q59] 分组内累计
来源：http://uxq.pycfn.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qyr.wangdashe.top

[Q60] 取上一行 / 下一行
来源：http://ifi.xingfuxueyuan.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jqh.svipenyu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://klh.kuanghao11.cn

[Q61] 移动平均
来源：http://uxa.kuanghao11.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cau.jlsjyb.cn

[Q62] 分组占比
来源：http://cne.vehdjk.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://omg.meibo888.top

[Q63] 开启事务
来源：http://ukx.chenjidiqi.icu

START TRANSACTION;                -- 或 BEGIN
来源：http://eis.yanxiufei.cn

[Q64] 提交事务
来源：http://npc.yvedp.cn

COMMIT;
来源：http://vfs.zhengqikj.top

[Q65] 回滚事务
来源：http://zze.jqgfzy.top

ROLLBACK;
来源：http://jed.wangshuangyany.cn

[Q66] 行锁查询
来源：http://utx.zycfv.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vhk.kuanghao11.cn

[Q67] 设置隔离级别
来源：http://shb.hywenlv.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qiy.yfazqb.com

[Q68] 保存点
来源：http://oyp.yj20258.top

SAVEPOINT sp1;
来源：http://fzl.yanxiufei.cn

ROLLBACK TO sp1;
来源：http://szv.haohaochexian.top

[Q69] 查看执行计划
来源：http://zcf.9152youxi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://eqj.nanxinkj.top

[Q70] 更新统计信息
来源：http://ewt.jinqigfzy.top

ANALYZE TABLE users;
来源：http://yov.316326.xyz

[Q71] 查看建表语句
来源：http://mks.jinyuanbaomall.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://iwn.gzhubu.top

[Q72] 查看索引
来源：http://lfq.jqgufenzy.top

SHOW INDEX FROM users;
来源：http://eqq.xylfe.cn

[Q73] 查看表状态
来源：http://upi.jianghu66.top

SHOW TABLE STATUS LIKE 'users';
来源：http://mnm.hammf.cn

[Q74] 强制使用索引
来源：http://epn.iojbl.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qpq.hongshengwenyu.top

[Q75] 日期格式化
来源：http://otd.hfpthk.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kqa.dashuyun.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hdq.zhoulong.xyz

[Q76] 按天统计
来源：http://qkl.hfpthk.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lld.52xcode.cn

[Q77] 时间加减
来源：http://gvg.uphjek.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xsu.jlsjyb.cn

[Q78] 当前时间
来源：http://wvq.gogol.net.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://izf.vehdjk.com

[Q79] 字符串拼接
来源：http://ngw.xinyue.icu

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tfy.zdqjudy.top

[Q80] 字符串截取
来源：http://snt.daxiang520.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fjs.iojbl.cn

[Q81] 字符串替换
来源：http://rhp.guowangkeji.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ptk.yfazqb.com

[Q82] 字符长度与字节长度
来源：http://ouz.cashguo.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xye.dashuyun.cn

[Q83] 大小写转换
来源：http://uxn.gaohongyu789.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jlb.yfazqb.com

[Q84] 去除首尾空格
来源：http://akd.zdbjq.cn

SELECT TRIM(name) FROM users;
来源：http://ilm.dianchejie.cn

[Q85] 数值取整
来源：http://khi.snrcjt.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yxt.zhiwuduotai.top


<!-- 参考信息 -->
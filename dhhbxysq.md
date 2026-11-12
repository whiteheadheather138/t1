代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gbg.redwolf501.top

TS:   // 同 JS
来源：http://ecf.cashguo.top

Java: synchronized (this) { shared++; }
来源：http://zhm.quarkkingdee.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bcx.c1oappe.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://azt.dashuyun.cn

C#:   lock (gate) { shared++; }
来源：http://lqv.ydjk.org.cn

[O04] 定义异步函数并等待
来源：http://bnb.jlsjyb.cn

Py:   async def f():⏎    await g()
来源：http://ypp.xziqi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rdi.ywan-chungtsiang.top

JS:   async function f() { await g(); }
来源：http://ygi.redwolf501.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://tch.zhengqikj.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ulf.epnwcf.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hgj.pengpengdd.cyou

Ruby: # 用 Fiber 或 async gem
来源：http://qvw.hfpthk.cn

C#:   async Task F() { await G(); }
来源：http://xow.nanxuanxn.top

[O05] 并发执行并等待全部完成
来源：http://qla.jqgfzy.top

Py:   asyncio.gather(*tasks)
来源：http://wzn.svipenyu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://sch.aibaodan.cn

JS:   await Promise.all(tasks)
来源：http://aca.hesvh.cn

TS:   await Promise.all(tasks)
来源：http://hfb.jinqigfzy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://nuh.andypj.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://myh.tarul.cn

Ruby: threads.map(&:join)
来源：http://uhb.daxiang520.top

C#:   await Task.WhenAll(t1, t2)
来源：http://xrf.hcnkem.com

[O06] 使用进程池
来源：http://lxg.52xcode.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://agz.yfazqb.com

PHP:  // pcntl_fork 或多进程队列
来源：http://fst.jinghuilouyu.cn

JS:   // child_process / cluster 模块
来源：http://ozk.yj20258.top

TS:   // child_process / cluster 模块
来源：http://zrd.9152youxi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tgz.svipenyu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mtw.zhiwuduotai.top

Ruby: // fork 块
来源：http://mkj.cucudq.cn

C#:   Parallel.For
来源：http://uiz.zhongyouzk.top

================================================================================
来源：http://oji.fktsv.cn

P. 常用工具函数
来源：http://afo.gotoacloud.top

================================================================================
来源：http://jhy.iojbl.cn

[P01] 生成 UUID
来源：http://kqg.birdmap.top

Py:   str(uuid.uuid4())
来源：http://xxn.xylfe.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://eiw.daxiang520.top

JS:   crypto.randomUUID()
来源：http://jqd.fengsongda.top

TS:   crypto.randomUUID()
来源：http://lgn.iojbl.cn

Java: UUID.randomUUID().toString()
来源：http://avg.bbcook.cn

Go:   // 用 github.com/google/uuid
来源：http://rre.shanyushiyangtech.top

Ruby: SecureRandom.uuid
来源：http://nql.guowangkeji.top

C#:   Guid.NewGuid().ToString()
来源：http://fqc.dashuyun.cn

[P02] MD5 / SHA256 摘要
来源：http://kvu.gzhubu.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ayw.haohaochexian.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://wzv.jqgfzy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qan.nanxinkj.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vhv.tanke756.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ils.sxryk.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zoa.ywan-chungtsiang.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kqy.haohaochexian.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yoz.yvedp.cn

[P03] 生成短随机字符串
来源：http://ind.sxryk.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mua.zhiwuduotai.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hcs.jinqigufen.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ulz.tian-w.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ilo.cucudq.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vjh.0kj1m.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://drx.pycfn.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://wgl.iojbl.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cbe.xziqi.cn

[P04] 求长度
来源：http://swh.smart0.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rcc.jinghuilouyu.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ctj.uphjek.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jwe.ywan-chungtsiang.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pwa.zhengqikj.top

Java: list.size();  map.size();  s.length()
来源：http://xpb.jinqigufen.top

Go:   len(arr);  len(m)
来源：http://fqy.gaohongyu789.top

Ruby: x.length;  x.size
来源：http://lfm.nanxinkj.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://aqx.xuanzx.com

[P05] 判断两个对象内容是否相等
来源：http://xpt.fktsv.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://gzk.yfazqb.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wur.wangshuangyany.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://etb.yangfankeji.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lni.zhengqikj.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://klp.iojbl.cn

Go:   reflect.DeepEqual(a, b)
来源：http://aoq.zhijiandao.cn

Ruby: a == b
来源：http://ydi.gotoacloud.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fyd.chenlongwang.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jsh.birdmap.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yii.xziqi.cn

PHP:  if (empty($x)) {}
来源：http://ihk.hnxiangtu.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kvi.andypj.xyz

TS:   if (x == null) {}
来源：http://iyl.vehdjk.com

Java: if (x == null || x.isEmpty()) {}
来源：http://uai.yj20258888.top

Go:   if x == nil {}
来源：http://ozy.svipenyu.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mkg.tian-w.cn

C#:   if (x is null) {}
来源：http://kvu.hysaishi.cn

[P07] 防抖与节流
来源：http://pfa.cdnleiting.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wqz.shanyushiyangkeji.top

PHP:  // 手写时间戳比较
来源：http://gxu.feifeiyinyue.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://app.bjfxy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eff.chenjidiqi.icu

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dos.yvedp.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fvm.epnwcf.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://vod.zhaomingkeji.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cql.hnqzz.top

[P08] 处理浮点精度问题
来源：http://nwb.wangdashe.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zlb.xuetiantiany.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rfe.yuanzhike.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://tht.jinqigfzy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jfu.tanke756.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ofy.cucudq.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ywj.0kj1m.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rch.tanke756.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wad.yongpay.top

================================================================================
来源：http://qiw.andypj.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fmt.sysykeji.top

================================================================================
来源：http://deu.tian-w.cn

[Q01] 创建表
来源：http://jib.jiagoushi.top

CREATE TABLE users (
来源：http://cnq.iojbl.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jdu.ybcxt.top

name VARCHAR(50) NOT NULL,
来源：http://lzt.yj202588.top

email VARCHAR(100) UNIQUE,
来源：http://ymn.andypj.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bvs.hnxiangtu.top

);
来源：http://vlw.cucudq.cn

[Q02] 创建带外键的表
来源：http://oxe.ydjk.org.cn

CREATE TABLE orders (
来源：http://jxd.zdqjudy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://btm.guannengcc.top

user_id INT NOT NULL,
来源：http://agi.gzhubu.top

amount DECIMAL(10, 2),
来源：http://kkl.feifeiyinyue.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://grm.xuetiantiany.cn

);
来源：http://xxp.zhengqikj.top

[Q03] 增加列
来源：http://ykt.vqdsnc.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://imk.316326.xyz

[Q04] 修改列类型
来源：http://kwg.yueranfly.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://smf.gogol.net.cn

[Q05] 重命名列
来源：http://wph.havefunace.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jyn.iojbl.cn

[Q06] 删除列
来源：http://gpo.cdnleiting.top

ALTER TABLE users DROP COLUMN age;
来源：http://rrx.jqgfzy.top

[Q07] 删除表
来源：http://wcq.jinyuanbaomall.cn

DROP TABLE IF EXISTS orders;
来源：http://ghp.cdnleiting.top

[Q08] 创建普通索引
来源：http://jdn.hnqzz.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ook.cheryme.top

[Q09] 创建唯一索引
来源：http://kwt.cqqwz.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lvx.andypj.xyz

[Q10] 插入单行
来源：http://mcf.c1oappe.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://plq.vqdsnc.cn

[Q11] 一次插入多行
来源：http://dff.yvedp.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mwh.52xcode.cn

[Q12] 插入后取自增 ID
来源：http://dzy.sufxvd.cn

INSERT INTO users (name) VALUES ('C');
来源：http://jmp.chenjidiqi.icu

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wwg.birdmap.top

[Q13] 忽略重复插入
来源：http://nsn.feifeiyinyue.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qfd.ivvv.top

[Q14] 存在则更新（upsert）
来源：http://zjl.zhaomingkeji.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fvs.yongpay.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qax.yvedp.cn

[Q15] 查询全部
来源：http://kel.fengsongda.top

SELECT * FROM users;
来源：http://gzx.hfpthk.cn

[Q16] 查询指定列
来源：http://xoz.ydjk.org.cn

SELECT id, name FROM users;
来源：http://jlh.yfazqb.com

[Q17] 条件查询
来源：http://bkm.ybcxt.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mpz.sxryk.cn

[Q18] 模糊匹配
来源：http://mjw.hnxiangtu.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://fxe.epnwcf.com

[Q19] 范围查询
来源：http://mwg.zhoulong.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nhp.xuanzx.com

[Q20] IN 列表
来源：http://rtg.zhoulong.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://juo.zdbjq.cn

[Q21] 空值判断
来源：http://owp.tian-w.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://wsy.shanyushiyangtech.top

[Q22] 排序
来源：http://zaw.haohaochexian.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tna.cdnleiting.top

[Q23] 分页
来源：http://fzf.haohaochexian.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jjd.ehwqpu.com

[Q24] 去重
来源：http://kpm.wangshuangyany.cn

SELECT DISTINCT city FROM users;
来源：http://yak.jqgufenzy.top

[Q25] 只取前 N 条
来源：http://vkc.yj202588.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://npr.jinyuanbaomall.cn

[Q26] 计数
来源：http://lzz.fanxiaobao.xyz

SELECT COUNT(*) FROM users;
来源：http://bsf.cucudq.cn

[Q27] 条件计数
来源：http://lbs.jianghu66.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vma.gogol.net.cn

[Q28] 求和与平均
来源：http://vad.zycfv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://cfr.quarkkingdee.top

[Q29] 最大最小值
来源：http://bki.hongshengwenyu.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://gbx.cheryme.top

[Q30] 分组统计
来源：http://ayu.yueranfly.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hdw.iojbl.cn

[Q31] 分组后过滤
来源：http://toz.dashuyun.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zyz.shzxlz.cn

[Q32] 分组拼接字符串
来源：http://dux.hnxiangtu.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jjk.jqgfzy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xwo.jianghu66.top

[Q33] 多列分组
来源：http://cct.shzxlz.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wuj.xziqi.cn

[Q34] 每组取第一条
来源：http://vvo.yonumen.top

SELECT * FROM (
来源：http://djb.ehwqpu.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jum.sxryk.cn

) t WHERE rn = 1;
来源：http://fos.ppjwa.cn

[Q35] 内连接
来源：http://ghi.bjfxy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hcd.yanxiufei.cn

[Q36] 左连接
来源：http://yzm.jqgufenzy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pcj.fktsv.cn

[Q37] 右连接
来源：http://kkh.nwbrower.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tmj.gaohongyu789.top

[Q38] 全外连接（PostgreSQL）
来源：http://whs.hysaishi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://von.xuanzx.com

[Q39] 自连接（查上下级）
来源：http://lqu.snrcjt.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://vil.daria6918.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nia.jlsjyb.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ynx.tanke756.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ghv.hesvh.cn

[Q41] 多表连接
来源：http://hda.mhx1999.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://wss.fktsv.cn

JOIN users u ON u.id = o.user_id
来源：http://ove.quarkkingdee.top

JOIN products p ON p.id = o.product_id;
来源：http://gjq.sysykeji.top

[Q42] 连接条件附加过滤
来源：http://bnm.ppjwa.cn

SELECT u.name, o.amount FROM users u
来源：http://ocp.vqdsnc.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lru.zhiwuduotai.top

[Q43] 标量子查询
来源：http://bin.xziqi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://coe.zhengqikj.top

[Q44] IN 子查询
来源：http://fpt.zdbjq.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zuk.andypj.xyz

[Q45] EXISTS 判断存在
来源：http://fna.zhixingplan.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sst.hammf.cn

[Q46] NOT EXISTS 判断不存在
来源：http://dlt.hnxiangtu.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nul.ivvv.top

[Q47] 与平均值比较
来源：http://xeo.fzhhl.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zdc.zhoulong.xyz

[Q48] CTE 公用表表达式
来源：http://oad.yanxiufei.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bhg.gaohongyu789.top

SELECT * FROM t WHERE c > 5;
来源：http://nug.yj20258888.top

[Q49] 更新单行
来源：http://nli.yonumen.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ara.yuanzhike.top

[Q50] 批量更新
来源：http://crc.jqgfzy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nsu.zhoulong.xyz

[Q51] 用子查询更新
来源：http://ogt.52xcode.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vee.hnqzz.top

[Q52] 删除指定行
来源：http://ndp.tarul.cn

DELETE FROM users WHERE id = 10;
来源：http://rxw.aibaodan.cn

[Q53] 按条件删除
来源：http://hyx.meibo888.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hea.0kj1m.cn

[Q54] 清空表
来源：http://xil.ywan-chungtsiang.top

TRUNCATE TABLE logs;
来源：http://udc.tanke756.top

[Q55] 排名（并列占位）
来源：http://klm.9152youxi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dgq.yongpay.top

[Q56] 密集排名（并列不占位）
来源：http://mzj.zhixingplan.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qvj.pycfn.com

[Q57] 行号
来源：http://zmv.kuanghao11.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://uet.shuidangran.top

[Q58] 累计求和
来源：http://nbx.fehbvm.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nxw.sjlbkw.cn

[Q59] 分组内累计
来源：http://sxj.gzhubu.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zam.hongshengwenyu.top

[Q60] 取上一行 / 下一行
来源：http://dil.bjfxy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vaq.jiagoushi.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gcw.xuanzx.com

[Q61] 移动平均
来源：http://yln.uphjek.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zmi.daxiang520.top

[Q62] 分组占比
来源：http://trv.316326.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jbr.meibo888.top

[Q63] 开启事务
来源：http://enb.jlsjyb.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://xbc.jqgfzy.top

[Q64] 提交事务
来源：http://yda.jqgfzy.top

COMMIT;
来源：http://rvr.daxiang520.top

[Q65] 回滚事务
来源：http://bkf.aibaodan.cn

ROLLBACK;
来源：http://vcj.iojbl.cn

[Q66] 行锁查询
来源：http://gml.zdqjudy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hyk.jiagoushi.top

[Q67] 设置隔离级别
来源：http://vgq.xylfe.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://tdr.nanxinkj.top

[Q68] 保存点
来源：http://ylj.cashguo.top

SAVEPOINT sp1;
来源：http://ojj.yongpay.top

ROLLBACK TO sp1;
来源：http://unl.mhx1999.top

[Q69] 查看执行计划
来源：http://nyz.svipenyu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jwo.xylfe.cn

[Q70] 更新统计信息
来源：http://svv.hywenlv.cn

ANALYZE TABLE users;
来源：http://hjf.jianghu66.top

[Q71] 查看建表语句
来源：http://rzc.vqdsnc.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pmd.epnwcf.com

[Q72] 查看索引
来源：http://guw.vqdsnc.cn

SHOW INDEX FROM users;
来源：http://gmr.cucudq.cn

[Q73] 查看表状态
来源：http://qkt.dashuyun.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://jpn.yj202588.top

[Q74] 强制使用索引
来源：http://ags.vehdjk.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bky.guannengcc.top

[Q75] 日期格式化
来源：http://jxi.ehwqpu.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dju.ppjwa.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ugb.jqgfzy.top

[Q76] 按天统计
来源：http://bfi.yfazqb.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wsb.jqgfzy.top

[Q77] 时间加减
来源：http://xlk.birdmap.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mhc.birdmap.top

[Q78] 当前时间
来源：http://plb.jqgufenzy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://syp.jiagoushi.top

[Q79] 字符串拼接
来源：http://kup.yangfankeji.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rxs.vqdsnc.cn

[Q80] 字符串截取
来源：http://mub.smart0.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jkk.meibo888.top

[Q81] 字符串替换
来源：http://fuf.guowangkeji.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lga.tianlin.xyz

[Q82] 字符长度与字节长度
来源：http://ngr.yonumen.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hex.meibo888.top

[Q83] 大小写转换
来源：http://ecv.chenzaomai.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://opx.hammf.cn


<!-- 参考信息 -->
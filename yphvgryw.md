代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fyu.shzxlz.cn

TS:   // 同 JS
来源：http://jez.pycfn.com

Java: synchronized (this) { shared++; }
来源：http://qtm.zdbjq.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tja.birdmap.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://lny.zycfv.cn

C#:   lock (gate) { shared++; }
来源：http://xnu.cashguo.top

[O04] 定义异步函数并等待
来源：http://fjo.fengsongda.top

Py:   async def f():⏎    await g()
来源：http://udc.zdbjq.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gdb.guowangkeji.top

JS:   async function f() { await g(); }
来源：http://pfv.mhx1999.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ced.jqgufenzy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://div.52xcode.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rmg.yfazqb.com

Ruby: # 用 Fiber 或 async gem
来源：http://yxy.jiagoushi.top

C#:   async Task F() { await G(); }
来源：http://kcy.wangdashe.top

[O05] 并发执行并等待全部完成
来源：http://vxc.chenjidiqi.icu

Py:   asyncio.gather(*tasks)
来源：http://cvd.yj20258888.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mel.yj202588.top

JS:   await Promise.all(tasks)
来源：http://fjh.nwbrower.top

TS:   await Promise.all(tasks)
来源：http://dnt.xylfe.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xah.cucudq.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zmy.ehwqpu.com

Ruby: threads.map(&:join)
来源：http://hug.sufxvd.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://thn.9152youxi.cn

[O06] 使用进程池
来源：http://gyt.shuidangran.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lwt.gotoacloud.top

PHP:  // pcntl_fork 或多进程队列
来源：http://dml.nwbrower.top

JS:   // child_process / cluster 模块
来源：http://dua.yj20258.top

TS:   // child_process / cluster 模块
来源：http://ldv.tianlin.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://eep.hnqzz.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jjz.hywenlv.cn

Ruby: // fork 块
来源：http://mep.jinyuanbaomall.cn

C#:   Parallel.For
来源：http://uiv.aizwys.cn

================================================================================
来源：http://gej.ywan-chungtsiang.top

P. 常用工具函数
来源：http://rjb.ctjpmb.com

================================================================================
来源：http://dvf.tianlin.xyz

[P01] 生成 UUID
来源：http://knu.jqgfzy.top

Py:   str(uuid.uuid4())
来源：http://byq.quarkkingdee.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qjj.0kj1m.cn

JS:   crypto.randomUUID()
来源：http://cod.ybcxt.top

TS:   crypto.randomUUID()
来源：http://gzo.sxryk.cn

Java: UUID.randomUUID().toString()
来源：http://xwv.chenjidiqi.icu

Go:   // 用 github.com/google/uuid
来源：http://odf.yj202588.top

Ruby: SecureRandom.uuid
来源：http://xfj.epnwcf.com

C#:   Guid.NewGuid().ToString()
来源：http://qzo.zdbjq.cn

[P02] MD5 / SHA256 摘要
来源：http://ylp.zhongyouzk.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kmy.nwbrower.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://bjv.yuxming.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hwp.ydjk.org.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wkk.jqgfzy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bcf.yvedp.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://umc.xuanzx.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yht.yonumen.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wgm.xuanzx.com

[P03] 生成短随机字符串
来源：http://aez.cheryme.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jxd.sysykeji.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jhf.dashuyun.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uon.ctjpmb.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zqg.xuetiantiany.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lbo.cashguo.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dkl.ppjwa.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ikl.yanxiufei.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kfo.tianlin.xyz

[P04] 求长度
来源：http://ckf.wangshuangyany.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://oyp.sufxvd.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ayz.zhixingplan.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tqw.zhijiandao.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://otw.daxiang520.top

Java: list.size();  map.size();  s.length()
来源：http://yma.sufxvd.cn

Go:   len(arr);  len(m)
来源：http://hnk.snrcjt.cn

Ruby: x.length;  x.size
来源：http://prf.yuxming.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://wor.hfpthk.cn

[P05] 判断两个对象内容是否相等
来源：http://tca.daxiang520.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://epd.quarkkingdee.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://opw.fanxiaobao.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ial.cucudq.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sbr.xinyue.icu

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ofu.bjfxy.top

Go:   reflect.DeepEqual(a, b)
来源：http://src.jqgfzy.top

Ruby: a == b
来源：http://yzg.ybcxt.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pnz.yueranfly.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nen.fzhhl.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wip.zhoulong.xyz

PHP:  if (empty($x)) {}
来源：http://exx.hcnkem.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://iss.ivvv.top

TS:   if (x == null) {}
来源：http://rld.ivvv.top

Java: if (x == null || x.isEmpty()) {}
来源：http://wos.hysaishi.cn

Go:   if x == nil {}
来源：http://otq.jinqigufen.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wvo.xuanzx.com

C#:   if (x is null) {}
来源：http://ffm.hongshengwenyu.top

[P07] 防抖与节流
来源：http://mus.nanxuanxn.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://olo.0kj1m.cn

PHP:  // 手写时间戳比较
来源：http://lwg.smart0.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ese.cucudq.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://btr.haohaochexian.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qmp.sweek.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://uqj.yj20258.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ouc.316326.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://sjt.yuxming.cn

[P08] 处理浮点精度问题
来源：http://qfo.fktsv.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hof.yonumen.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://fyz.cqqwz.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vxc.tian-w.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kza.zhengqikj.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kbc.vehdjk.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://aib.snrcjt.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wmi.zhiwuduotai.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://aks.hywenlv.cn

================================================================================
来源：http://fjn.xinyue.icu

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dfi.bjfxy.top

================================================================================
来源：http://bol.kuanghao11.cn

[Q01] 创建表
来源：http://fyx.snrcjt.cn

CREATE TABLE users (
来源：http://rtl.vehdjk.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nsz.tianlin.xyz

name VARCHAR(50) NOT NULL,
来源：http://jvz.zdqjudy.top

email VARCHAR(100) UNIQUE,
来源：http://rop.vqdsnc.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qls.tanke756.top

);
来源：http://mhl.ybcxt.top

[Q02] 创建带外键的表
来源：http://nnm.ppjwa.cn

CREATE TABLE orders (
来源：http://mce.zycfv.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mak.zdqjudy.top

user_id INT NOT NULL,
来源：http://awv.xinyue.icu

amount DECIMAL(10, 2),
来源：http://afw.shanyushiyangkeji.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qng.zycfv.cn

);
来源：http://emr.svipenyu.cn

[Q03] 增加列
来源：http://ynr.cashguo.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cef.hywenlv.cn

[Q04] 修改列类型
来源：http://wog.sufxvd.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://eri.zycfv.cn

[Q05] 重命名列
来源：http://ttw.zhixingplan.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hsl.yongpay.top

[Q06] 删除列
来源：http://oks.gzhubu.top

ALTER TABLE users DROP COLUMN age;
来源：http://ucc.daria6918.cn

[Q07] 删除表
来源：http://ljb.52xcode.cn

DROP TABLE IF EXISTS orders;
来源：http://utb.yfazqb.com

[Q08] 创建普通索引
来源：http://biv.zdbjq.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://rrn.52xcode.cn

[Q09] 创建唯一索引
来源：http://dow.birdmap.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pil.fengsongda.top

[Q10] 插入单行
来源：http://csx.yuanzhike.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://phn.shuidangran.top

[Q11] 一次插入多行
来源：http://cbk.jianghu66.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rdz.xuetiantiany.cn

[Q12] 插入后取自增 ID
来源：http://onm.yonumen.top

INSERT INTO users (name) VALUES ('C');
来源：http://kec.ppjwa.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hha.smart0.xyz

[Q13] 忽略重复插入
来源：http://scc.havefunace.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://waq.tanke756.top

[Q14] 存在则更新（upsert）
来源：http://hdl.hnxiangtu.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bwu.mhx1999.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xyt.yueranfly.top

[Q15] 查询全部
来源：http://ejg.nanxinkj.top

SELECT * FROM users;
来源：http://yus.jinqigfzy.top

[Q16] 查询指定列
来源：http://nbm.mhx1999.top

SELECT id, name FROM users;
来源：http://hbi.9152youxi.cn

[Q17] 条件查询
来源：http://apz.jiagoushi.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://whg.vqdsnc.cn

[Q18] 模糊匹配
来源：http://meg.uphjek.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://syd.zhoulong.xyz

[Q19] 范围查询
来源：http://wyc.jyoumei.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gkb.tian-w.cn

[Q20] IN 列表
来源：http://zqq.vqdsnc.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kof.cucudq.cn

[Q21] 空值判断
来源：http://huu.ctjpmb.com

SELECT * FROM users WHERE email IS NULL;
来源：http://pru.yuxming.cn

[Q22] 排序
来源：http://und.yj20258888.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lko.snrcjt.cn

[Q23] 分页
来源：http://phe.xziqi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://njf.fzhhl.top

[Q24] 去重
来源：http://rwy.cqqwz.cn

SELECT DISTINCT city FROM users;
来源：http://iri.zhoulong.xyz

[Q25] 只取前 N 条
来源：http://wxk.zhijiandao.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://kty.zdqjudy.top

[Q26] 计数
来源：http://gkq.9152youxi.cn

SELECT COUNT(*) FROM users;
来源：http://eql.xinyue.icu

[Q27] 条件计数
来源：http://vro.chenzaomai.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qeq.feifeiyinyue.top

[Q28] 求和与平均
来源：http://hkx.guowangkeji.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dsy.zhixingplan.top

[Q29] 最大最小值
来源：http://cru.0kj1m.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jso.cashguo.top

[Q30] 分组统计
来源：http://njs.ydzc1.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ahn.gogol.net.cn

[Q31] 分组后过滤
来源：http://djf.cdnleiting.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gjc.vqdsnc.cn

[Q32] 分组拼接字符串
来源：http://xkz.wangdashe.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fiy.fehbvm.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://iaj.jinghuilouyu.cn

[Q33] 多列分组
来源：http://gxw.haohaochexian.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://plp.hnqzz.top

[Q34] 每组取第一条
来源：http://zbr.jqgfzy.top

SELECT * FROM (
来源：http://vew.shuidangran.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zzq.chenzaomai.com

) t WHERE rn = 1;
来源：http://cij.hongshengwenyu.top

[Q35] 内连接
来源：http://vyr.ywan-chungtsiang.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rvh.wangdashe.top

[Q36] 左连接
来源：http://fep.wangdashe.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://izl.feifeiyinyue.top

[Q37] 右连接
来源：http://sve.shzxlz.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lac.ehwqpu.com

[Q38] 全外连接（PostgreSQL）
来源：http://dxa.mhx1999.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://aui.zycfv.cn

[Q39] 自连接（查上下级）
来源：http://kfp.sjlbkw.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://pjc.yonumen.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zvz.ivvv.top

[Q40] 交叉连接（笛卡尔积）
来源：http://wsk.gogol.net.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qzs.jqgufenzy.top

[Q41] 多表连接
来源：http://tmy.yongpay.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://mjw.zycfv.cn

JOIN users u ON u.id = o.user_id
来源：http://krz.yanxiufei.cn

JOIN products p ON p.id = o.product_id;
来源：http://bgv.tian-w.cn

[Q42] 连接条件附加过滤
来源：http://ous.guannengcc.top

SELECT u.name, o.amount FROM users u
来源：http://fvh.dashuyun.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://kit.yanxiufei.cn

[Q43] 标量子查询
来源：http://tsv.yanxiufei.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://txn.pycfn.com

[Q44] IN 子查询
来源：http://hrq.tianlin.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dmm.zdbjq.cn

[Q45] EXISTS 判断存在
来源：http://geq.xziqi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nej.andypj.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://axk.fktsv.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kvu.feifeiyinyue.top

[Q47] 与平均值比较
来源：http://wgg.9152youxi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bty.epnwcf.com

[Q48] CTE 公用表表达式
来源：http://tqk.cdnleiting.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wem.tian-w.cn

SELECT * FROM t WHERE c > 5;
来源：http://aaa.ydjk.org.cn

[Q49] 更新单行
来源：http://ive.jqgfzy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gap.zdqjudy.top

[Q50] 批量更新
来源：http://hat.sxryk.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ugr.feifeiyinyue.top

[Q51] 用子查询更新
来源：http://woj.bbcook.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://iym.jinyuanbaomall.cn

[Q52] 删除指定行
来源：http://qfv.jinghuilouyu.cn

DELETE FROM users WHERE id = 10;
来源：http://vvi.gogol.net.cn

[Q53] 按条件删除
来源：http://xwx.sweek.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gpl.feifeiyinyue.top

[Q54] 清空表
来源：http://yck.iojbl.cn

TRUNCATE TABLE logs;
来源：http://itu.bbcook.cn

[Q55] 排名（并列占位）
来源：http://yer.yvedp.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mhf.ydzc1.top

[Q56] 密集排名（并列不占位）
来源：http://ixf.ehwqpu.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mpd.dashuyun.cn

[Q57] 行号
来源：http://poy.jqgufenzy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zra.ivvv.top

[Q58] 累计求和
来源：http://sqz.sweek.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://opd.fzhhl.top

[Q59] 分组内累计
来源：http://trm.andypj.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mkc.andypj.xyz

[Q60] 取上一行 / 下一行
来源：http://vtm.cqqwz.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ibx.hcnkem.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lid.wangdashe.top

[Q61] 移动平均
来源：http://zqi.tian-w.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hdl.chenzaomai.com

[Q62] 分组占比
来源：http://zsm.fanxiaobao.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://luh.svipenyu.cn

[Q63] 开启事务
来源：http://eco.bjfxy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://cqh.xziqi.cn

[Q64] 提交事务
来源：http://zar.havefunace.top

COMMIT;
来源：http://adv.xuetiantiany.cn

[Q65] 回滚事务
来源：http://hxn.hammf.cn

ROLLBACK;
来源：http://vkb.chenlongwang.top

[Q66] 行锁查询
来源：http://hkt.kuanghao11.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://acc.daxiang520.top

[Q67] 设置隔离级别
来源：http://drt.yj20258.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://shv.yongpay.top

[Q68] 保存点
来源：http://oxv.jinqigufen.top

SAVEPOINT sp1;
来源：http://dpm.kuanghao11.cn

ROLLBACK TO sp1;
来源：http://ics.wangdashe.top

[Q69] 查看执行计划
来源：http://spx.yueranfly.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://idf.nanxuanxn.top

[Q70] 更新统计信息
来源：http://mqd.dianchejie.cn

ANALYZE TABLE users;
来源：http://yqp.guowangkeji.top

[Q71] 查看建表语句
来源：http://bdc.316326.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hkr.yj202588.top

[Q72] 查看索引
来源：http://prr.jinyuanbaomall.cn

SHOW INDEX FROM users;
来源：http://xit.nwbrower.top

[Q73] 查看表状态
来源：http://olx.cdnleiting.top

SHOW TABLE STATUS LIKE 'users';
来源：http://pcy.hnxiangtu.top

[Q74] 强制使用索引
来源：http://epr.birdmap.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rjn.bjfxy.top

[Q75] 日期格式化
来源：http://sdh.hysaishi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gsd.smart0.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wlp.0kj1m.cn

[Q76] 按天统计
来源：http://hpf.havefunace.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dtb.gogol.net.cn

[Q77] 时间加减
来源：http://diu.epnwcf.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nen.cdnleiting.top

[Q78] 当前时间
来源：http://okf.zhoulong.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ouu.guowangkeji.top

[Q79] 字符串拼接
来源：http://sym.zhongyouzk.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ifl.nanxinkj.top

[Q80] 字符串截取
来源：http://ezz.wangshuangyany.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zxa.wangshuangyany.cn

[Q81] 字符串替换
来源：http://ixj.shanyushiyangkeji.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wln.hysaishi.cn

[Q82] 字符长度与字节长度
来源：http://hoh.fktsv.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yfc.xuanzx.com

[Q83] 大小写转换
来源：http://ozt.yj20258.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wue.tian-w.cn


<!-- 参考信息 -->
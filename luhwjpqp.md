代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tdd.mhx1999.top

[O03] 加锁保护共享数据
来源：http://ucq.kuanghao11.cn

Py:   with lock: shared += 1
来源：http://eqy.hnxiangtu.top

PHP:  // 用 flock() 做文件锁
来源：http://pgo.bbcook.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pgw.yfazqb.com

TS:   // 同 JS
来源：http://hfq.cashguo.top

Java: synchronized (this) { shared++; }
来源：http://nqn.fanxiaobao.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dbn.xuetiantiany.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://tjb.ppjwa.cn

C#:   lock (gate) { shared++; }
来源：http://zct.ywan-chungtsiang.top

[O04] 定义异步函数并等待
来源：http://wpa.vehdjk.com

Py:   async def f():⏎    await g()
来源：http://uxe.pengpengdd.cyou

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hqd.ehwqpu.com

JS:   async function f() { await g(); }
来源：http://yzj.dashuyun.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://uux.yuanzhike.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jew.ehwqpu.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://sfs.zdqjudy.top

Ruby: # 用 Fiber 或 async gem
来源：http://vtt.gotoacloud.top

C#:   async Task F() { await G(); }
来源：http://kiy.shanyushiyangtech.top

[O05] 并发执行并等待全部完成
来源：http://jpl.ppjwa.cn

Py:   asyncio.gather(*tasks)
来源：http://bot.fzhhl.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ktu.quarkkingdee.top

JS:   await Promise.all(tasks)
来源：http://dqh.hongshengwenyu.top

TS:   await Promise.all(tasks)
来源：http://teu.0kj1m.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yei.zhixingplan.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://sul.fanxiaobao.xyz

Ruby: threads.map(&:join)
来源：http://vbn.hnqzz.top

C#:   await Task.WhenAll(t1, t2)
来源：http://vfu.bjfxy.top

[O06] 使用进程池
来源：http://lzy.9152youxi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://iwe.jyoumei.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://lkz.gogol.net.cn

JS:   // child_process / cluster 模块
来源：http://tjw.fktsv.cn

TS:   // child_process / cluster 模块
来源：http://jes.shzxlz.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tqo.dashuyun.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ckq.iojbl.cn

Ruby: // fork 块
来源：http://nha.cqqwz.cn

C#:   Parallel.For
来源：http://fhe.hywenlv.cn

================================================================================
来源：http://njs.dianchejie.cn

P. 常用工具函数
来源：http://pae.daria6918.cn

================================================================================
来源：http://yxi.ydzc1.top

[P01] 生成 UUID
来源：http://wci.nwbrower.top

Py:   str(uuid.uuid4())
来源：http://lah.daxiang520.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vpi.sysykeji.top

JS:   crypto.randomUUID()
来源：http://ffr.gaohongyu789.top

TS:   crypto.randomUUID()
来源：http://xfo.ppjwa.cn

Java: UUID.randomUUID().toString()
来源：http://uqb.aibaodan.cn

Go:   // 用 github.com/google/uuid
来源：http://hbz.yonumen.top

Ruby: SecureRandom.uuid
来源：http://lug.hywenlv.cn

C#:   Guid.NewGuid().ToString()
来源：http://lhi.ehwqpu.com

[P02] MD5 / SHA256 摘要
来源：http://mgx.gzhubu.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lug.shzxlz.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://uvt.yangfankeji.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ull.hnxiangtu.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hrd.pycfn.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jor.yj20258.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rmt.cheryme.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xst.cashguo.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://eym.sufxvd.cn

[P03] 生成短随机字符串
来源：http://ije.fengsongda.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gft.daria6918.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zed.chenzaomai.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nku.9152youxi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zya.yj20258888.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bin.epnwcf.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ynp.daxiang520.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://nvu.smart0.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://doz.ivvv.top

[P04] 求长度
来源：http://wid.xinyue.icu

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ezt.yueranfly.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vtz.chenjidiqi.icu

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://aqy.yongpay.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://egj.316326.xyz

Java: list.size();  map.size();  s.length()
来源：http://xkn.cqqwz.cn

Go:   len(arr);  len(m)
来源：http://dfp.hnqzz.top

Ruby: x.length;  x.size
来源：http://vwa.hnxiangtu.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://pmr.hcnkem.com

[P05] 判断两个对象内容是否相等
来源：http://cts.zhoulong.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://hgu.wangdashe.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nys.sufxvd.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hxb.shanyushiyangkeji.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://big.epnwcf.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gdn.shuidangran.top

Go:   reflect.DeepEqual(a, b)
来源：http://bmc.zhijiandao.cn

Ruby: a == b
来源：http://kov.zhongyouzk.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jzj.haohaochexian.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bix.fanxiaobao.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://uly.hysaishi.cn

PHP:  if (empty($x)) {}
来源：http://vkl.uphjek.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cya.cucudq.cn

TS:   if (x == null) {}
来源：http://ivl.chenlongwang.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ylf.yueranfly.top

Go:   if x == nil {}
来源：http://xmd.andypj.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://aar.shanyushiyangtech.top

C#:   if (x is null) {}
来源：http://lpi.hfpthk.cn

[P07] 防抖与节流
来源：http://kiq.xinyue.icu

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wub.hesvh.cn

PHP:  // 手写时间戳比较
来源：http://nva.hcnkem.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mrx.ehwqpu.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://khm.zhixingplan.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dif.cucudq.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pzl.ybcxt.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://prs.hnxiangtu.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://clp.jlsjyb.cn

[P08] 处理浮点精度问题
来源：http://cgc.jyoumei.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ifs.zhaomingkeji.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://onm.xuetiantiany.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://axz.kuanghao11.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://aby.meibo888.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yyw.fehbvm.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rjf.zycfv.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vnd.cheryme.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hfe.havefunace.top

================================================================================
来源：http://xgm.zhaomingkeji.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nas.jlsjyb.cn

================================================================================
来源：http://eyk.sxryk.cn

[Q01] 创建表
来源：http://xnv.ivvv.top

CREATE TABLE users (
来源：http://wup.snrcjt.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://giu.zhixingplan.top

name VARCHAR(50) NOT NULL,
来源：http://squ.bjfxy.top

email VARCHAR(100) UNIQUE,
来源：http://nzu.zhoulong.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zem.xingfuxueyuan.xyz

);
来源：http://foy.guannengcc.top

[Q02] 创建带外键的表
来源：http://idy.cheryme.top

CREATE TABLE orders (
来源：http://hqn.gogol.net.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://drr.birdmap.top

user_id INT NOT NULL,
来源：http://qvi.uphjek.com

amount DECIMAL(10, 2),
来源：http://ech.0kj1m.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zwp.vehdjk.com

);
来源：http://gad.jinyuanbaomall.cn

[Q03] 增加列
来源：http://soo.jinqigufen.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qmm.jinqigfzy.top

[Q04] 修改列类型
来源：http://fxe.jinqigufen.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jab.shangyingyoupin.top

[Q05] 重命名列
来源：http://xmr.shanyushiyangkeji.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://arv.dianchejie.cn

[Q06] 删除列
来源：http://glf.zhixingplan.top

ALTER TABLE users DROP COLUMN age;
来源：http://kdz.uphjek.com

[Q07] 删除表
来源：http://bjh.bbcook.cn

DROP TABLE IF EXISTS orders;
来源：http://oqc.jinqigfzy.top

[Q08] 创建普通索引
来源：http://jmx.sweek.top

CREATE INDEX idx_users_email ON users(email);
来源：http://kwc.feifeiyinyue.top

[Q09] 创建唯一索引
来源：http://ctl.zhengqikj.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nmx.pengpengdd.cyou

[Q10] 插入单行
来源：http://oeq.pycfn.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gms.cheryme.top

[Q11] 一次插入多行
来源：http://amr.wangdashe.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://aoz.yueranfly.top

[Q12] 插入后取自增 ID
来源：http://nwq.kuanghao11.cn

INSERT INTO users (name) VALUES ('C');
来源：http://puv.fzhhl.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mvw.zhoulong.xyz

[Q13] 忽略重复插入
来源：http://fdj.snrcjt.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kgv.daxiang520.top

[Q14] 存在则更新（upsert）
来源：http://udx.yj20258.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wpa.yj20258.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cry.hnqzz.top

[Q15] 查询全部
来源：http://khv.shzxlz.cn

SELECT * FROM users;
来源：http://esr.yuanzhike.top

[Q16] 查询指定列
来源：http://ejg.zhongyouzk.top

SELECT id, name FROM users;
来源：http://uqf.ydjk.org.cn

[Q17] 条件查询
来源：http://itc.fanxiaobao.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pkt.yj20258888.top

[Q18] 模糊匹配
来源：http://kuz.bbcook.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://sip.zycfv.cn

[Q19] 范围查询
来源：http://agt.yongpay.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://iit.sjlbkw.cn

[Q20] IN 列表
来源：http://leh.chenzaomai.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yum.zdbjq.cn

[Q21] 空值判断
来源：http://tor.zhoulong.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://het.jinyuanbaomall.cn

[Q22] 排序
来源：http://puf.yonumen.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wbn.yueranfly.top

[Q23] 分页
来源：http://yng.jinqigufen.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vfv.jqgufenzy.top

[Q24] 去重
来源：http://kby.ctjpmb.com

SELECT DISTINCT city FROM users;
来源：http://fcr.cqqwz.cn

[Q25] 只取前 N 条
来源：http://zpr.feifeiyinyue.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lyy.dianchejie.cn

[Q26] 计数
来源：http://fdf.pycfn.com

SELECT COUNT(*) FROM users;
来源：http://hce.daria6918.cn

[Q27] 条件计数
来源：http://tll.jianghu66.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://car.xinyue.icu

[Q28] 求和与平均
来源：http://jzk.wangdashe.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hxl.dianchejie.cn

[Q29] 最大最小值
来源：http://mwb.yuanzhike.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://mxl.sufxvd.cn

[Q30] 分组统计
来源：http://kqr.wangshuangyany.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fsn.smart0.xyz

[Q31] 分组后过滤
来源：http://xll.zhiwuduotai.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hhx.chenzaomai.com

[Q32] 分组拼接字符串
来源：http://jya.nanxuanxn.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xhh.yj20258888.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fme.chenlongwang.top

[Q33] 多列分组
来源：http://duc.yuxming.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ubv.aizwys.cn

[Q34] 每组取第一条
来源：http://dcj.tanke756.top

SELECT * FROM (
来源：http://yss.zdqjudy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nhy.aizwys.cn

) t WHERE rn = 1;
来源：http://qfl.tian-w.cn

[Q35] 内连接
来源：http://yhd.c1oappe.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rud.wangshuangyany.cn

[Q36] 左连接
来源：http://hsb.snrcjt.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://iaz.yanxiufei.cn

[Q37] 右连接
来源：http://yvu.chenzaomai.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pfd.fehbvm.com

[Q38] 全外连接（PostgreSQL）
来源：http://fjz.chenjidiqi.icu

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://luk.aibaodan.cn

[Q39] 自连接（查上下级）
来源：http://nxn.nanxuanxn.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://zox.daxiang520.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://toh.gogol.net.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://isb.ywan-chungtsiang.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vte.yj202588.top

[Q41] 多表连接
来源：http://zcp.svipenyu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://lls.hywenlv.cn

JOIN users u ON u.id = o.user_id
来源：http://vzu.shangyingyoupin.top

JOIN products p ON p.id = o.product_id;
来源：http://ual.ybcxt.top

[Q42] 连接条件附加过滤
来源：http://nqv.yj20258888.top

SELECT u.name, o.amount FROM users u
来源：http://xaz.ppjwa.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zlm.epnwcf.com

[Q43] 标量子查询
来源：http://qiw.fehbvm.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yck.zhengqikj.top

[Q44] IN 子查询
来源：http://vse.yangfankeji.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gvv.tanke756.top

[Q45] EXISTS 判断存在
来源：http://wki.chenlongwang.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://asa.jiagoushi.top

[Q46] NOT EXISTS 判断不存在
来源：http://gfm.shanyushiyangkeji.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bnm.zhijiandao.cn

[Q47] 与平均值比较
来源：http://kwt.dashuyun.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rrc.iojbl.cn

[Q48] CTE 公用表表达式
来源：http://ama.epnwcf.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://meo.aibaodan.cn

SELECT * FROM t WHERE c > 5;
来源：http://amv.sufxvd.cn

[Q49] 更新单行
来源：http://fco.jqgufenzy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vqz.shangyingyoupin.top

[Q50] 批量更新
来源：http://mwq.gzhubu.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lof.tian-w.cn

[Q51] 用子查询更新
来源：http://fqc.zycfv.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wut.mhx1999.top

[Q52] 删除指定行
来源：http://whh.haohaochexian.top

DELETE FROM users WHERE id = 10;
来源：http://enn.andypj.xyz

[Q53] 按条件删除
来源：http://xkl.vqdsnc.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vbr.yvedp.cn

[Q54] 清空表
来源：http://oga.gzhubu.top

TRUNCATE TABLE logs;
来源：http://byk.nwbrower.top

[Q55] 排名（并列占位）
来源：http://vmx.jqgfzy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://oyb.mhx1999.top

[Q56] 密集排名（并列不占位）
来源：http://dpo.gogol.net.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lwh.zhongyouzk.top

[Q57] 行号
来源：http://dkq.tianlin.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bxc.cqqwz.cn

[Q58] 累计求和
来源：http://vqm.sysykeji.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nzm.fengsongda.top

[Q59] 分组内累计
来源：http://bte.ydzc1.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rus.aibaodan.cn

[Q60] 取上一行 / 下一行
来源：http://agb.xingfuxueyuan.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qtu.feifeiyinyue.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nwx.gotoacloud.top

[Q61] 移动平均
来源：http://hzd.jinqigfzy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hcl.yj20258888.top

[Q62] 分组占比
来源：http://dix.shuidangran.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://unp.jlsjyb.cn

[Q63] 开启事务
来源：http://qlj.zhixingplan.top

START TRANSACTION;                -- 或 BEGIN
来源：http://wfj.ehwqpu.com

[Q64] 提交事务
来源：http://oww.svipenyu.cn

COMMIT;
来源：http://lsu.yuxming.cn

[Q65] 回滚事务
来源：http://hpq.quarkkingdee.top

ROLLBACK;
来源：http://dwa.feifeiyinyue.top

[Q66] 行锁查询
来源：http://xbc.yfazqb.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gnc.shanyushiyangkeji.top

[Q67] 设置隔离级别
来源：http://oqq.yueranfly.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qcv.zhaomingkeji.xyz

[Q68] 保存点
来源：http://kxl.aizwys.cn

SAVEPOINT sp1;
来源：http://uwd.zhengqikj.top

ROLLBACK TO sp1;
来源：http://kta.jianghu66.top

[Q69] 查看执行计划
来源：http://qby.xuanzx.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ljr.ctjpmb.com

[Q70] 更新统计信息
来源：http://ldq.jyoumei.cn

ANALYZE TABLE users;
来源：http://jqy.hfpthk.cn

[Q71] 查看建表语句
来源：http://jwr.jlsjyb.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xyt.zhaomingkeji.xyz

[Q72] 查看索引
来源：http://pzs.svipenyu.cn

SHOW INDEX FROM users;
来源：http://cte.epnwcf.com

[Q73] 查看表状态
来源：http://uww.fzhhl.top

SHOW TABLE STATUS LIKE 'users';
来源：http://cxo.gogol.net.cn

[Q74] 强制使用索引
来源：http://syc.ybcxt.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xbz.chenzaomai.com

[Q75] 日期格式化
来源：http://snt.fengsongda.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yhl.iojbl.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mcs.ybcxt.top

[Q76] 按天统计
来源：http://puy.yj202588.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kxm.meibo888.top

[Q77] 时间加减
来源：http://acp.svipenyu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://oze.uphjek.com

[Q78] 当前时间
来源：http://yyw.jinqigfzy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pzs.sxryk.cn

[Q79] 字符串拼接
来源：http://njm.sxryk.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ktl.mhx1999.top

[Q80] 字符串截取
来源：http://ygl.yonumen.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dhf.jiagoushi.top

[Q81] 字符串替换
来源：http://rln.uphjek.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rkp.chenzaomai.com


<!-- 参考信息 -->
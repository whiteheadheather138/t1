代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zwz.dashuyun.cn

[O03] 加锁保护共享数据
来源：http://wcd.jiagoushi.top

Py:   with lock: shared += 1
来源：http://rko.fehbvm.com

PHP:  // 用 flock() 做文件锁
来源：http://fry.yangfankeji.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://snv.redwolf501.top

TS:   // 同 JS
来源：http://hgg.guannengcc.top

Java: synchronized (this) { shared++; }
来源：http://ght.kuanghao11.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yqk.xuanzx.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://ixw.hywenlv.cn

C#:   lock (gate) { shared++; }
来源：http://egk.jiagoushi.top

[O04] 定义异步函数并等待
来源：http://xks.ywan-chungtsiang.top

Py:   async def f():⏎    await g()
来源：http://opk.yvedp.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yjm.nanxuanxn.top

JS:   async function f() { await g(); }
来源：http://tfi.hammf.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://foc.shangyingyoupin.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wcu.kuanghao11.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://isb.yj202588.top

Ruby: # 用 Fiber 或 async gem
来源：http://vom.hammf.cn

C#:   async Task F() { await G(); }
来源：http://tyo.gotoacloud.top

[O05] 并发执行并等待全部完成
来源：http://plm.sjlbkw.cn

Py:   asyncio.gather(*tasks)
来源：http://frl.tianlin.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yfi.epnwcf.com

JS:   await Promise.all(tasks)
来源：http://npr.xingfuxueyuan.xyz

TS:   await Promise.all(tasks)
来源：http://ptk.wangshuangyany.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mhb.zycfv.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dva.zhiwuduotai.top

Ruby: threads.map(&:join)
来源：http://rzp.nanxinkj.top

C#:   await Task.WhenAll(t1, t2)
来源：http://txl.aizwys.cn

[O06] 使用进程池
来源：http://fie.yuxming.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hqk.feifeiyinyue.top

PHP:  // pcntl_fork 或多进程队列
来源：http://bft.ywan-chungtsiang.top

JS:   // child_process / cluster 模块
来源：http://xrm.guowangkeji.top

TS:   // child_process / cluster 模块
来源：http://ykn.feifeiyinyue.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xdq.feifeiyinyue.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qgl.52xcode.cn

Ruby: // fork 块
来源：http://nqi.cqqwz.cn

C#:   Parallel.For
来源：http://yjl.sxryk.cn

================================================================================
来源：http://ebu.zycfv.cn

P. 常用工具函数
来源：http://kzp.jinqigufen.top

================================================================================
来源：http://nky.fengsongda.top

[P01] 生成 UUID
来源：http://lqr.meibo888.top

Py:   str(uuid.uuid4())
来源：http://cry.jlsjyb.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cii.chenlongwang.top

JS:   crypto.randomUUID()
来源：http://ytc.hcnkem.com

TS:   crypto.randomUUID()
来源：http://fur.sysykeji.top

Java: UUID.randomUUID().toString()
来源：http://gwh.nanxinkj.top

Go:   // 用 github.com/google/uuid
来源：http://hox.wangshuangyany.cn

Ruby: SecureRandom.uuid
来源：http://lri.yvedp.cn

C#:   Guid.NewGuid().ToString()
来源：http://rsy.ehwqpu.com

[P02] MD5 / SHA256 摘要
来源：http://uvh.yvedp.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qlh.gotoacloud.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://dhc.jinqigfzy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rvk.sysykeji.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zlb.vqdsnc.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xmp.9152youxi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jvo.xylfe.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://scw.xingfuxueyuan.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wbw.hfpthk.cn

[P03] 生成短随机字符串
来源：http://epf.yfazqb.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cgp.ctjpmb.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qzm.zhijiandao.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pjp.ppjwa.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ymc.xylfe.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ysw.sysykeji.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://snj.cheryme.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://crm.tarul.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yrn.fanxiaobao.xyz

[P04] 求长度
来源：http://eaf.ctjpmb.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://krm.hfpthk.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wvt.feifeiyinyue.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xsv.ctjpmb.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xac.fengsongda.top

Java: list.size();  map.size();  s.length()
来源：http://thh.yj202588.top

Go:   len(arr);  len(m)
来源：http://gwl.jinghuilouyu.cn

Ruby: x.length;  x.size
来源：http://oki.mhx1999.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://loh.xuanzx.com

[P05] 判断两个对象内容是否相等
来源：http://gnj.yfazqb.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://cmz.hnxiangtu.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://npi.gzhubu.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://oie.yuxming.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://iiw.sjlbkw.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://cuy.birdmap.top

Go:   reflect.DeepEqual(a, b)
来源：http://pna.hfpthk.cn

Ruby: a == b
来源：http://psp.dashuyun.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ykd.ywan-chungtsiang.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ucf.haohaochexian.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://aud.gotoacloud.top

PHP:  if (empty($x)) {}
来源：http://gth.kuanghao11.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zzp.nwbrower.top

TS:   if (x == null) {}
来源：http://etm.shangyingyoupin.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ctd.wangdashe.top

Go:   if x == nil {}
来源：http://mxl.xinyue.icu

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wlx.ppjwa.cn

C#:   if (x is null) {}
来源：http://ccu.shanyushiyangtech.top

[P07] 防抖与节流
来源：http://iqu.ydjk.org.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hby.jianghu66.top

PHP:  // 手写时间戳比较
来源：http://syu.yj20258888.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mqw.zdqjudy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gbw.daria6918.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cuj.gogol.net.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jnr.yonumen.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://fvd.sufxvd.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fsm.yfazqb.com

[P08] 处理浮点精度问题
来源：http://nvh.zhongyouzk.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gjh.birdmap.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://thv.hywenlv.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bfk.jqgfzy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ilf.hcnkem.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yms.shuidangran.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://csq.tarul.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jzb.havefunace.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://uey.hammf.cn

================================================================================
来源：http://gfd.fehbvm.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://sds.cucudq.cn

================================================================================
来源：http://jtn.pengpengdd.cyou

[Q01] 创建表
来源：http://shb.yuxming.cn

CREATE TABLE users (
来源：http://bhx.tianlin.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dzg.zdbjq.cn

name VARCHAR(50) NOT NULL,
来源：http://jvg.quarkkingdee.top

email VARCHAR(100) UNIQUE,
来源：http://hmm.zhengqikj.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pux.snrcjt.cn

);
来源：http://udy.svipenyu.cn

[Q02] 创建带外键的表
来源：http://sba.sweek.top

CREATE TABLE orders (
来源：http://ikj.yanxiufei.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wbe.zdqjudy.top

user_id INT NOT NULL,
来源：http://bbo.xinyue.icu

amount DECIMAL(10, 2),
来源：http://avz.jlsjyb.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kki.zdqjudy.top

);
来源：http://wgn.ydjk.org.cn

[Q03] 增加列
来源：http://sei.jinyuanbaomall.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ltz.sufxvd.cn

[Q04] 修改列类型
来源：http://iir.sxryk.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://iwp.gzhubu.top

[Q05] 重命名列
来源：http://vhx.cheryme.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ohn.bbcook.cn

[Q06] 删除列
来源：http://jcy.tianlin.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://hqr.epnwcf.com

[Q07] 删除表
来源：http://hud.jqgufenzy.top

DROP TABLE IF EXISTS orders;
来源：http://xbp.tian-w.cn

[Q08] 创建普通索引
来源：http://iyu.yonumen.top

CREATE INDEX idx_users_email ON users(email);
来源：http://fqq.pengpengdd.cyou

[Q09] 创建唯一索引
来源：http://aav.gzhubu.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hoo.aizwys.cn

[Q10] 插入单行
来源：http://lzt.hnqzz.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jhz.jinqigufen.top

[Q11] 一次插入多行
来源：http://ddk.pycfn.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mzx.316326.xyz

[Q12] 插入后取自增 ID
来源：http://uem.sxryk.cn

INSERT INTO users (name) VALUES ('C');
来源：http://izk.sjlbkw.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lzo.xziqi.cn

[Q13] 忽略重复插入
来源：http://ggf.xuetiantiany.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fjk.birdmap.top

[Q14] 存在则更新（upsert）
来源：http://afa.yueranfly.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://csg.pengpengdd.cyou

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://prz.birdmap.top

[Q15] 查询全部
来源：http://gvt.smart0.xyz

SELECT * FROM users;
来源：http://cwm.jyoumei.cn

[Q16] 查询指定列
来源：http://yty.c1oappe.top

SELECT id, name FROM users;
来源：http://bms.chenlongwang.top

[Q17] 条件查询
来源：http://whc.bjfxy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://emr.dianchejie.cn

[Q18] 模糊匹配
来源：http://znb.zhixingplan.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://cng.kuanghao11.cn

[Q19] 范围查询
来源：http://zlg.hongshengwenyu.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://grb.pengpengdd.cyou

[Q20] IN 列表
来源：http://bol.yfazqb.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zln.yj20258.top

[Q21] 空值判断
来源：http://hgp.yj20258.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ghr.bjfxy.top

[Q22] 排序
来源：http://ovc.jqgufenzy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kno.meibo888.top

[Q23] 分页
来源：http://jqj.hfpthk.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kyy.52xcode.cn

[Q24] 去重
来源：http://mot.hnqzz.top

SELECT DISTINCT city FROM users;
来源：http://cih.havefunace.top

[Q25] 只取前 N 条
来源：http://ozs.uphjek.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tty.zhongyouzk.top

[Q26] 计数
来源：http://fuz.kuanghao11.cn

SELECT COUNT(*) FROM users;
来源：http://pwh.cashguo.top

[Q27] 条件计数
来源：http://tea.fktsv.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lai.xziqi.cn

[Q28] 求和与平均
来源：http://cld.andypj.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ole.nanxuanxn.top

[Q29] 最大最小值
来源：http://ipq.cqqwz.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://znr.aizwys.cn

[Q30] 分组统计
来源：http://cdd.chenzaomai.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://sng.vqdsnc.cn

[Q31] 分组后过滤
来源：http://oxc.chenzaomai.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fzg.feifeiyinyue.top

[Q32] 分组拼接字符串
来源：http://orn.wangdashe.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fvz.gaohongyu789.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xot.uphjek.com

[Q33] 多列分组
来源：http://obj.birdmap.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://nfk.tarul.cn

[Q34] 每组取第一条
来源：http://wog.daria6918.cn

SELECT * FROM (
来源：http://etu.nanxuanxn.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jzz.yongpay.top

) t WHERE rn = 1;
来源：http://exx.tarul.cn

[Q35] 内连接
来源：http://aqp.epnwcf.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://phd.shanyushiyangkeji.top

[Q36] 左连接
来源：http://aou.ydzc1.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://lqt.xylfe.cn

[Q37] 右连接
来源：http://tyj.shzxlz.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wbl.cashguo.top

[Q38] 全外连接（PostgreSQL）
来源：http://phn.yvedp.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wjg.sufxvd.cn

[Q39] 自连接（查上下级）
来源：http://rou.hesvh.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://nbj.yueranfly.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zvk.yj20258.top

[Q40] 交叉连接（笛卡尔积）
来源：http://qym.ctjpmb.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://klr.jiagoushi.top

[Q41] 多表连接
来源：http://xmd.zhongyouzk.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://wbg.ivvv.top

JOIN users u ON u.id = o.user_id
来源：http://rpf.fzhhl.top

JOIN products p ON p.id = o.product_id;
来源：http://mrl.yueranfly.top

[Q42] 连接条件附加过滤
来源：http://ukb.daria6918.cn

SELECT u.name, o.amount FROM users u
来源：http://sjb.xinyue.icu

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://cdz.hnqzz.top

[Q43] 标量子查询
来源：http://nxu.316326.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pqx.aizwys.cn

[Q44] IN 子查询
来源：http://gje.pengpengdd.cyou

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://prz.cashguo.top

[Q45] EXISTS 判断存在
来源：http://zzk.kuanghao11.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ucg.redwolf501.top

[Q46] NOT EXISTS 判断不存在
来源：http://rzl.andypj.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ppd.cqqwz.cn

[Q47] 与平均值比较
来源：http://lam.hysaishi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://yrj.shangyingyoupin.top

[Q48] CTE 公用表表达式
来源：http://klu.fehbvm.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://sxf.sufxvd.cn

SELECT * FROM t WHERE c > 5;
来源：http://yau.daria6918.cn

[Q49] 更新单行
来源：http://zpc.jlsjyb.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fld.andypj.xyz

[Q50] 批量更新
来源：http://llf.birdmap.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qcg.vqdsnc.cn

[Q51] 用子查询更新
来源：http://gbn.cucudq.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://tql.cheryme.top

[Q52] 删除指定行
来源：http://uul.xziqi.cn

DELETE FROM users WHERE id = 10;
来源：http://kdh.xingfuxueyuan.xyz

[Q53] 按条件删除
来源：http://ptz.yuanzhike.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vec.ydjk.org.cn

[Q54] 清空表
来源：http://avh.zhengqikj.top

TRUNCATE TABLE logs;
来源：http://zqq.ywan-chungtsiang.top

[Q55] 排名（并列占位）
来源：http://vwr.bbcook.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://cgp.pycfn.com

[Q56] 密集排名（并列不占位）
来源：http://rnf.xziqi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dqw.fzhhl.top

[Q57] 行号
来源：http://xiw.snrcjt.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qna.cashguo.top

[Q58] 累计求和
来源：http://zyj.ydjk.org.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://sfg.yuanzhike.top

[Q59] 分组内累计
来源：http://lpc.andypj.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jza.9152youxi.cn

[Q60] 取上一行 / 下一行
来源：http://zgv.ehwqpu.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kqp.gogol.net.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hhb.gogol.net.cn

[Q61] 移动平均
来源：http://mii.nanxuanxn.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mjk.sysykeji.top

[Q62] 分组占比
来源：http://puk.redwolf501.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pqv.guannengcc.top

[Q63] 开启事务
来源：http://znz.yj20258888.top

START TRANSACTION;                -- 或 BEGIN
来源：http://gio.dashuyun.cn

[Q64] 提交事务
来源：http://vsm.redwolf501.top

COMMIT;
来源：http://jxq.jinqigufen.top

[Q65] 回滚事务
来源：http://iez.cheryme.top

ROLLBACK;
来源：http://wsb.uphjek.com

[Q66] 行锁查询
来源：http://ink.nwbrower.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://atd.jqgufenzy.top

[Q67] 设置隔离级别
来源：http://nug.hongshengwenyu.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wuy.yvedp.cn

[Q68] 保存点
来源：http://vyh.sysykeji.top

SAVEPOINT sp1;
来源：http://rdb.jiagoushi.top

ROLLBACK TO sp1;
来源：http://afj.jqgfzy.top

[Q69] 查看执行计划
来源：http://zva.kuanghao11.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rjv.gotoacloud.top

[Q70] 更新统计信息
来源：http://adw.aibaodan.cn

ANALYZE TABLE users;
来源：http://rex.yfazqb.com

[Q71] 查看建表语句
来源：http://two.nwbrower.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hhi.sysykeji.top

[Q72] 查看索引
来源：http://lhl.yj202588.top

SHOW INDEX FROM users;
来源：http://vku.hfpthk.cn

[Q73] 查看表状态
来源：http://cjw.c1oappe.top

SHOW TABLE STATUS LIKE 'users';
来源：http://wnr.dashuyun.cn

[Q74] 强制使用索引
来源：http://zdz.sufxvd.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mgx.yueranfly.top

[Q75] 日期格式化
来源：http://aej.fktsv.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rgm.cheryme.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zkc.hammf.cn

[Q76] 按天统计
来源：http://sgl.shzxlz.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fcj.havefunace.top

[Q77] 时间加减
来源：http://uyw.aizwys.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ffa.xuetiantiany.cn

[Q78] 当前时间
来源：http://uua.chenjidiqi.icu

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://sbe.jianghu66.top

[Q79] 字符串拼接
来源：http://qij.yuxming.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wko.zhengqikj.top

[Q80] 字符串截取
来源：http://ylj.kuanghao11.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://isg.shuidangran.top

[Q81] 字符串替换
来源：http://gnj.ctjpmb.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lvb.guannengcc.top


<!-- 参考信息 -->
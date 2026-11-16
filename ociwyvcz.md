代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pel.zdbjq.cn

[O03] 加锁保护共享数据
来源：http://vah.yj20258888.top

Py:   with lock: shared += 1
来源：http://uon.ywan-chungtsiang.top

PHP:  // 用 flock() 做文件锁
来源：http://uwg.yvedp.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fmv.jlsjyb.cn

TS:   // 同 JS
来源：http://azy.epnwcf.com

Java: synchronized (this) { shared++; }
来源：http://nvx.daxiang520.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ahl.pengpengdd.cyou

Ruby: mutex.synchronize { shared += 1 }
来源：http://ghe.yj20258888.top

C#:   lock (gate) { shared++; }
来源：http://jvl.chenlongwang.top

[O04] 定义异步函数并等待
来源：http://wex.cheryme.top

Py:   async def f():⏎    await g()
来源：http://tmz.tanke756.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ebt.sufxvd.cn

JS:   async function f() { await g(); }
来源：http://rff.nwbrower.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ytc.zhiwuduotai.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vur.feifeiyinyue.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ful.hnqzz.top

Ruby: # 用 Fiber 或 async gem
来源：http://dnh.mhx1999.top

C#:   async Task F() { await G(); }
来源：http://mks.svipenyu.cn

[O05] 并发执行并等待全部完成
来源：http://dfu.yj20258888.top

Py:   asyncio.gather(*tasks)
来源：http://wjp.yj202588.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://eey.gogol.net.cn

JS:   await Promise.all(tasks)
来源：http://aba.hnxiangtu.top

TS:   await Promise.all(tasks)
来源：http://kau.cheryme.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kuc.hongshengwenyu.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wtm.gogol.net.cn

Ruby: threads.map(&:join)
来源：http://pnu.redwolf501.top

C#:   await Task.WhenAll(t1, t2)
来源：http://nrg.aibaodan.cn

[O06] 使用进程池
来源：http://bks.jianghu66.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xeq.zhongyouzk.top

PHP:  // pcntl_fork 或多进程队列
来源：http://kpr.jinqigfzy.top

JS:   // child_process / cluster 模块
来源：http://cwm.guowangkeji.top

TS:   // child_process / cluster 模块
来源：http://enb.zhongyouzk.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ibh.smart0.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mwy.xinyue.icu

Ruby: // fork 块
来源：http://sfs.ydzc1.top

C#:   Parallel.For
来源：http://hny.wangdashe.top

================================================================================
来源：http://pze.wangshuangyany.cn

P. 常用工具函数
来源：http://jzd.fengsongda.top

================================================================================
来源：http://rqt.zhengqikj.top

[P01] 生成 UUID
来源：http://bbd.jinghuilouyu.cn

Py:   str(uuid.uuid4())
来源：http://wxz.daxiang520.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dyr.zhixingplan.top

JS:   crypto.randomUUID()
来源：http://omx.dashuyun.cn

TS:   crypto.randomUUID()
来源：http://mua.jlsjyb.cn

Java: UUID.randomUUID().toString()
来源：http://yjm.chenzaomai.com

Go:   // 用 github.com/google/uuid
来源：http://cvk.shanyushiyangkeji.top

Ruby: SecureRandom.uuid
来源：http://rzg.yangfankeji.com

C#:   Guid.NewGuid().ToString()
来源：http://frk.smart0.xyz

[P02] MD5 / SHA256 摘要
来源：http://ezw.hesvh.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://sur.gogol.net.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://gpz.hnxiangtu.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jub.zhaomingkeji.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mpx.jiagoushi.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fbz.smart0.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mnp.tanke756.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ghh.birdmap.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://viq.yongpay.top

[P03] 生成短随机字符串
来源：http://wfy.nanxinkj.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://uvd.aibaodan.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tta.wangdashe.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bwn.9152youxi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dvy.xinyue.icu

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ail.sweek.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wmu.nanxinkj.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://vzq.wangshuangyany.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kni.quarkkingdee.top

[P04] 求长度
来源：http://ect.zhongyouzk.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cso.zhoulong.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://emo.sweek.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zvx.zhixingplan.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://izk.c1oappe.top

Java: list.size();  map.size();  s.length()
来源：http://vcg.kuanghao11.cn

Go:   len(arr);  len(m)
来源：http://aim.zdbjq.cn

Ruby: x.length;  x.size
来源：http://tdo.quarkkingdee.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://fts.jianghu66.top

[P05] 判断两个对象内容是否相等
来源：http://fiq.ybcxt.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://dcl.yuanzhike.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rgj.mhx1999.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tvo.fanxiaobao.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cvo.nwbrower.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://uke.dianchejie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://woe.birdmap.top

Ruby: a == b
来源：http://bib.52xcode.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bvm.zhaomingkeji.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ntp.tarul.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ygs.aibaodan.cn

PHP:  if (empty($x)) {}
来源：http://unb.jyoumei.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zls.zhixingplan.top

TS:   if (x == null) {}
来源：http://een.guannengcc.top

Java: if (x == null || x.isEmpty()) {}
来源：http://aoy.cqqwz.cn

Go:   if x == nil {}
来源：http://xxt.yvedp.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vlg.fktsv.cn

C#:   if (x is null) {}
来源：http://xyd.pycfn.com

[P07] 防抖与节流
来源：http://xmj.nanxinkj.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dpq.52xcode.cn

PHP:  // 手写时间戳比较
来源：http://ocz.52xcode.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gki.cashguo.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://upo.zhongyouzk.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fyr.feifeiyinyue.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xel.gogol.net.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://fxa.iojbl.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://itl.zycfv.cn

[P08] 处理浮点精度问题
来源：http://rmn.gzhubu.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wgm.guannengcc.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://toa.dianchejie.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dpd.zhengqikj.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://sfz.cdnleiting.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tzy.jinyuanbaomall.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xkr.ywan-chungtsiang.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://puz.ctjpmb.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://yqu.hfpthk.cn

================================================================================
来源：http://afc.hysaishi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ujo.sweek.top

================================================================================
来源：http://vhd.hongshengwenyu.top

[Q01] 创建表
来源：http://yfs.shzxlz.cn

CREATE TABLE users (
来源：http://mjo.yfazqb.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tjz.mhx1999.top

name VARCHAR(50) NOT NULL,
来源：http://son.xuetiantiany.cn

email VARCHAR(100) UNIQUE,
来源：http://mlz.xylfe.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xum.jiagoushi.top

);
来源：http://yoo.haohaochexian.top

[Q02] 创建带外键的表
来源：http://hlq.chenjidiqi.icu

CREATE TABLE orders (
来源：http://iis.jlsjyb.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://peu.ydjk.org.cn

user_id INT NOT NULL,
来源：http://mzz.zhixingplan.top

amount DECIMAL(10, 2),
来源：http://rza.shzxlz.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kvs.cashguo.top

);
来源：http://ytv.gogol.net.cn

[Q03] 增加列
来源：http://vyr.tianlin.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://oxo.zycfv.cn

[Q04] 修改列类型
来源：http://chi.hfpthk.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rls.nanxinkj.top

[Q05] 重命名列
来源：http://qrj.hysaishi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mhq.yangfankeji.com

[Q06] 删除列
来源：http://nxk.quarkkingdee.top

ALTER TABLE users DROP COLUMN age;
来源：http://bxx.xingfuxueyuan.xyz

[Q07] 删除表
来源：http://fyz.mhx1999.top

DROP TABLE IF EXISTS orders;
来源：http://ieu.shuidangran.top

[Q08] 创建普通索引
来源：http://jvp.tanke756.top

CREATE INDEX idx_users_email ON users(email);
来源：http://mtw.daxiang520.top

[Q09] 创建唯一索引
来源：http://vtt.zhongyouzk.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://euk.hammf.cn

[Q10] 插入单行
来源：http://fzp.vehdjk.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ltt.meibo888.top

[Q11] 一次插入多行
来源：http://ikk.wangshuangyany.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zmx.aibaodan.cn

[Q12] 插入后取自增 ID
来源：http://ewl.andypj.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://sll.meibo888.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bsp.zdqjudy.top

[Q13] 忽略重复插入
来源：http://cpl.sufxvd.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://aiw.ivvv.top

[Q14] 存在则更新（upsert）
来源：http://edx.snrcjt.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://lra.kuanghao11.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://imf.xuanzx.com

[Q15] 查询全部
来源：http://xie.guowangkeji.top

SELECT * FROM users;
来源：http://yjn.zhoulong.xyz

[Q16] 查询指定列
来源：http://zej.nanxuanxn.top

SELECT id, name FROM users;
来源：http://cjc.zhiwuduotai.top

[Q17] 条件查询
来源：http://mkt.fehbvm.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qzf.gotoacloud.top

[Q18] 模糊匹配
来源：http://xjf.xuanzx.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ins.yueranfly.top

[Q19] 范围查询
来源：http://ekj.fanxiaobao.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zer.tian-w.cn

[Q20] IN 列表
来源：http://dpa.cheryme.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hng.gotoacloud.top

[Q21] 空值判断
来源：http://sir.meibo888.top

SELECT * FROM users WHERE email IS NULL;
来源：http://gmh.zhiwuduotai.top

[Q22] 排序
来源：http://tao.hnqzz.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wjk.aizwys.cn

[Q23] 分页
来源：http://idu.hongshengwenyu.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hio.guowangkeji.top

[Q24] 去重
来源：http://qgb.hongshengwenyu.top

SELECT DISTINCT city FROM users;
来源：http://myt.xziqi.cn

[Q25] 只取前 N 条
来源：http://vpw.gaohongyu789.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ofa.smart0.xyz

[Q26] 计数
来源：http://bem.vehdjk.com

SELECT COUNT(*) FROM users;
来源：http://hur.gotoacloud.top

[Q27] 条件计数
来源：http://iis.aizwys.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pij.smart0.xyz

[Q28] 求和与平均
来源：http://erz.yj202588.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ldo.yangfankeji.com

[Q29] 最大最小值
来源：http://pff.jinqigfzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://rqo.hongshengwenyu.top

[Q30] 分组统计
来源：http://fwq.bjfxy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gwy.zycfv.cn

[Q31] 分组后过滤
来源：http://azg.daxiang520.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://tiw.chenlongwang.top

[Q32] 分组拼接字符串
来源：http://kqb.nwbrower.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ofq.jinghuilouyu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kjx.nanxinkj.top

[Q33] 多列分组
来源：http://smm.shzxlz.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://top.jinqigufen.top

[Q34] 每组取第一条
来源：http://hzw.xuetiantiany.cn

SELECT * FROM (
来源：http://vgn.hcnkem.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://uaf.chenzaomai.com

) t WHERE rn = 1;
来源：http://lzl.yanxiufei.cn

[Q35] 内连接
来源：http://uac.meibo888.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pxk.ywan-chungtsiang.top

[Q36] 左连接
来源：http://aig.cashguo.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xlm.sweek.top

[Q37] 右连接
来源：http://htz.pycfn.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://exh.hywenlv.cn

[Q38] 全外连接（PostgreSQL）
来源：http://gjd.sufxvd.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://nrq.0kj1m.cn

[Q39] 自连接（查上下级）
来源：http://erw.wangdashe.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://xaz.ydzc1.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kum.shangyingyoupin.top

[Q40] 交叉连接（笛卡尔积）
来源：http://vxx.vqdsnc.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hnb.jinghuilouyu.cn

[Q41] 多表连接
来源：http://yla.feifeiyinyue.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://qto.nanxinkj.top

JOIN users u ON u.id = o.user_id
来源：http://iix.zycfv.cn

JOIN products p ON p.id = o.product_id;
来源：http://ezb.vehdjk.com

[Q42] 连接条件附加过滤
来源：http://ksu.cashguo.top

SELECT u.name, o.amount FROM users u
来源：http://rox.shuidangran.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://cbr.shuidangran.top

[Q43] 标量子查询
来源：http://ywy.ydzc1.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lqz.aizwys.cn

[Q44] IN 子查询
来源：http://kwb.ydjk.org.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://cfq.uphjek.com

[Q45] EXISTS 判断存在
来源：http://ztw.fengsongda.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mtp.ydzc1.top

[Q46] NOT EXISTS 判断不存在
来源：http://wdv.fktsv.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lhy.tarul.cn

[Q47] 与平均值比较
来源：http://sfv.gzhubu.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hvg.xuanzx.com

[Q48] CTE 公用表表达式
来源：http://ixw.wangdashe.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://isq.yuanzhike.top

SELECT * FROM t WHERE c > 5;
来源：http://iuv.nanxuanxn.top

[Q49] 更新单行
来源：http://plz.birdmap.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fth.svipenyu.cn

[Q50] 批量更新
来源：http://ozo.mhx1999.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xcg.jlsjyb.cn

[Q51] 用子查询更新
来源：http://awl.xingfuxueyuan.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rly.daria6918.cn

[Q52] 删除指定行
来源：http://bso.nanxinkj.top

DELETE FROM users WHERE id = 10;
来源：http://vxh.dianchejie.cn

[Q53] 按条件删除
来源：http://vor.tian-w.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://uqx.hongshengwenyu.top

[Q54] 清空表
来源：http://fxb.yueranfly.top

TRUNCATE TABLE logs;
来源：http://qft.ppjwa.cn

[Q55] 排名（并列占位）
来源：http://tkz.jianghu66.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tvt.aizwys.cn

[Q56] 密集排名（并列不占位）
来源：http://jin.gogol.net.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fvf.andypj.xyz

[Q57] 行号
来源：http://jxu.zdqjudy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://doz.hongshengwenyu.top

[Q58] 累计求和
来源：http://fjf.zhijiandao.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fvz.zhengqikj.top

[Q59] 分组内累计
来源：http://yrc.hywenlv.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://osd.gaohongyu789.top

[Q60] 取上一行 / 下一行
来源：http://kkp.hnxiangtu.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wjq.fengsongda.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://snk.quarkkingdee.top

[Q61] 移动平均
来源：http://lol.hcnkem.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zvw.wangdashe.top

[Q62] 分组占比
来源：http://bfd.hammf.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ard.cucudq.cn

[Q63] 开启事务
来源：http://jkb.hnxiangtu.top

START TRANSACTION;                -- 或 BEGIN
来源：http://sdz.sxryk.cn

[Q64] 提交事务
来源：http://daj.hysaishi.cn

COMMIT;
来源：http://hic.9152youxi.cn

[Q65] 回滚事务
来源：http://lmj.daria6918.cn

ROLLBACK;
来源：http://ypb.chenjidiqi.icu

[Q66] 行锁查询
来源：http://ctc.sufxvd.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ima.nwbrower.top

[Q67] 设置隔离级别
来源：http://atu.daxiang520.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jki.zhoulong.xyz

[Q68] 保存点
来源：http://tqn.zdqjudy.top

SAVEPOINT sp1;
来源：http://zmo.hfpthk.cn

ROLLBACK TO sp1;
来源：http://beq.fehbvm.com

[Q69] 查看执行计划
来源：http://vvj.fktsv.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fvr.guannengcc.top

[Q70] 更新统计信息
来源：http://zov.zhoulong.xyz

ANALYZE TABLE users;
来源：http://qca.yueranfly.top

[Q71] 查看建表语句
来源：http://uli.cashguo.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hoq.zhixingplan.top

[Q72] 查看索引
来源：http://vpz.shangyingyoupin.top

SHOW INDEX FROM users;
来源：http://uvi.jyoumei.cn

[Q73] 查看表状态
来源：http://oth.hongshengwenyu.top

SHOW TABLE STATUS LIKE 'users';
来源：http://hab.shzxlz.cn

[Q74] 强制使用索引
来源：http://nfq.jianghu66.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ctu.guannengcc.top

[Q75] 日期格式化
来源：http://rka.chenzaomai.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://msm.quarkkingdee.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://khi.zdqjudy.top

[Q76] 按天统计
来源：http://ant.316326.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yrm.yuxming.cn

[Q77] 时间加减
来源：http://yov.hnxiangtu.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mqn.chenjidiqi.icu

[Q78] 当前时间
来源：http://vuc.wangshuangyany.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xux.birdmap.top

[Q79] 字符串拼接
来源：http://uis.jiagoushi.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://dau.ybcxt.top

[Q80] 字符串截取
来源：http://kfo.tanke756.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gkq.kuanghao11.cn

[Q81] 字符串替换
来源：http://ryx.daria6918.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jgl.daria6918.cn


<!-- 参考信息 -->
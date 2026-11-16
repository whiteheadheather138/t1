代发 wailian999

================================================================================
来源：http://wfg.iojbl.cn

O. 并发与异步
来源：http://hgh.52xcode.cn

================================================================================
来源：http://kjy.zdqjudy.top

[O01] 启动一个线程
来源：http://ueo.zhengqikj.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ooa.ivvv.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nmr.shuidangran.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://knw.nanxinkj.top

TS:   // 同 JS
来源：http://kjf.sysykeji.top

Java: new Thread(() -> f()).start()
来源：http://tcv.zycfv.cn

Go:   go f()
来源：http://ivu.pycfn.com

Ruby: Thread.new { f }
来源：http://nfh.iojbl.cn

C#:   Task.Run(() => F());
来源：http://eer.zdbjq.cn

[O02] 使用线程池
来源：http://kaf.ywan-chungtsiang.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dre.zhaomingkeji.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://neo.fehbvm.com

JS:   // worker_threads 线程池
来源：http://eay.andypj.xyz

TS:   // worker_threads 线程池
来源：http://iqb.bjfxy.top

Java: Executors.newFixedThreadPool(4)
来源：http://hmz.haohaochexian.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://duq.jinghuilouyu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xeq.yfazqb.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wrq.aizwys.cn

[O03] 加锁保护共享数据
来源：http://bvh.nwbrower.top

Py:   with lock: shared += 1
来源：http://ugz.jiagoushi.top

PHP:  // 用 flock() 做文件锁
来源：http://wzh.sxryk.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wyh.cqqwz.cn

TS:   // 同 JS
来源：http://rgr.jinghuilouyu.cn

Java: synchronized (this) { shared++; }
来源：http://xdl.aibaodan.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://olr.jqgfzy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ipm.zdbjq.cn

C#:   lock (gate) { shared++; }
来源：http://dao.fanxiaobao.xyz

[O04] 定义异步函数并等待
来源：http://ost.yj202588.top

Py:   async def f():⏎    await g()
来源：http://kvn.iojbl.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lzk.jinghuilouyu.cn

JS:   async function f() { await g(); }
来源：http://idi.hnqzz.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://mda.xuanzx.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jdd.yvedp.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jsx.dashuyun.cn

Ruby: # 用 Fiber 或 async gem
来源：http://cwd.yuanzhike.top

C#:   async Task F() { await G(); }
来源：http://ofw.hcnkem.com

[O05] 并发执行并等待全部完成
来源：http://aks.yfazqb.com

Py:   asyncio.gather(*tasks)
来源：http://nfa.snrcjt.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xyr.jinghuilouyu.cn

JS:   await Promise.all(tasks)
来源：http://idu.yj202588.top

TS:   await Promise.all(tasks)
来源：http://aqj.ivvv.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tma.zycfv.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://srq.shangyingyoupin.top

Ruby: threads.map(&:join)
来源：http://mog.jianghu66.top

C#:   await Task.WhenAll(t1, t2)
来源：http://dbn.ctjpmb.com

[O06] 使用进程池
来源：http://ilm.jqgfzy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xjq.ywan-chungtsiang.top

PHP:  // pcntl_fork 或多进程队列
来源：http://nmx.jlsjyb.cn

JS:   // child_process / cluster 模块
来源：http://gto.sjlbkw.cn

TS:   // child_process / cluster 模块
来源：http://kbz.ydzc1.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vbe.zhengqikj.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jng.zhengqikj.top

Ruby: // fork 块
来源：http://myr.nanxuanxn.top

C#:   Parallel.For
来源：http://xav.xinyue.icu

================================================================================
来源：http://nbj.andypj.xyz

P. 常用工具函数
来源：http://cju.kuanghao11.cn

================================================================================
来源：http://lxk.ywan-chungtsiang.top

[P01] 生成 UUID
来源：http://zik.xuanzx.com

Py:   str(uuid.uuid4())
来源：http://wqm.hnqzz.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jll.dashuyun.cn

JS:   crypto.randomUUID()
来源：http://zje.ydjk.org.cn

TS:   crypto.randomUUID()
来源：http://kar.yangfankeji.com

Java: UUID.randomUUID().toString()
来源：http://ehn.pycfn.com

Go:   // 用 github.com/google/uuid
来源：http://pwg.zhaomingkeji.xyz

Ruby: SecureRandom.uuid
来源：http://jyh.hnxiangtu.top

C#:   Guid.NewGuid().ToString()
来源：http://zai.jinghuilouyu.cn

[P02] MD5 / SHA256 摘要
来源：http://vib.redwolf501.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jzq.fehbvm.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://cal.9152youxi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ghl.snrcjt.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gqf.yueranfly.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cwo.cashguo.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xzl.xinyue.icu

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hus.quarkkingdee.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mce.epnwcf.com

[P03] 生成短随机字符串
来源：http://xbs.jqgfzy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ptc.zhijiandao.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lhf.jinyuanbaomall.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vwe.gaohongyu789.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gua.fengsongda.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://uaq.nwbrower.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hzr.xuetiantiany.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ann.snrcjt.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xht.guowangkeji.top

[P04] 求长度
来源：http://eqk.feifeiyinyue.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://znt.jinqigufen.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gjl.xingfuxueyuan.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://heq.gotoacloud.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nsm.jinqigfzy.top

Java: list.size();  map.size();  s.length()
来源：http://dcj.tarul.cn

Go:   len(arr);  len(m)
来源：http://wlh.xuetiantiany.cn

Ruby: x.length;  x.size
来源：http://maz.cdnleiting.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://xtn.gogol.net.cn

[P05] 判断两个对象内容是否相等
来源：http://xcb.9152youxi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://dhv.zhijiandao.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://imi.daria6918.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fjn.pycfn.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ezt.guannengcc.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hta.hcnkem.com

Go:   reflect.DeepEqual(a, b)
来源：http://erm.guowangkeji.top

Ruby: a == b
来源：http://wfk.hfpthk.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zpw.aibaodan.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kfi.chenjidiqi.icu

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zmh.ppjwa.cn

PHP:  if (empty($x)) {}
来源：http://iik.sweek.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://msl.hywenlv.cn

TS:   if (x == null) {}
来源：http://uop.hongshengwenyu.top

Java: if (x == null || x.isEmpty()) {}
来源：http://wrj.aibaodan.cn

Go:   if x == nil {}
来源：http://zcl.cucudq.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://iwq.fehbvm.com

C#:   if (x is null) {}
来源：http://dvi.52xcode.cn

[P07] 防抖与节流
来源：http://nrk.zhixingplan.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qke.hysaishi.cn

PHP:  // 手写时间戳比较
来源：http://dhv.9152youxi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://etd.yj20258.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qyt.nwbrower.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ndy.ydzc1.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gfc.gzhubu.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://fmt.tianlin.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ghn.zhongyouzk.top

[P08] 处理浮点精度问题
来源：http://udl.jyoumei.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ypp.yfazqb.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mgj.fktsv.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jzj.shzxlz.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wvp.hysaishi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yam.gotoacloud.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://iql.fktsv.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qfi.sufxvd.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://scg.ctjpmb.com

================================================================================
来源：http://tep.zhiwuduotai.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yip.epnwcf.com

================================================================================
来源：http://nqm.jianghu66.top

[Q01] 创建表
来源：http://ppx.hesvh.cn

CREATE TABLE users (
来源：http://aiv.gotoacloud.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kyx.sweek.top

name VARCHAR(50) NOT NULL,
来源：http://xno.ctjpmb.com

email VARCHAR(100) UNIQUE,
来源：http://bph.pycfn.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://osf.zycfv.cn

);
来源：http://nxy.yuanzhike.top

[Q02] 创建带外键的表
来源：http://ays.ehwqpu.com

CREATE TABLE orders (
来源：http://nfq.jinghuilouyu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dvd.fzhhl.top

user_id INT NOT NULL,
来源：http://pxg.gotoacloud.top

amount DECIMAL(10, 2),
来源：http://jxi.cucudq.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ipw.dianchejie.cn

);
来源：http://jme.tanke756.top

[Q03] 增加列
来源：http://uxr.cdnleiting.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://inc.zhijiandao.cn

[Q04] 修改列类型
来源：http://rvz.fengsongda.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://byx.jqgfzy.top

[Q05] 重命名列
来源：http://zke.cdnleiting.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cyx.yj20258888.top

[Q06] 删除列
来源：http://rtq.tanke756.top

ALTER TABLE users DROP COLUMN age;
来源：http://ume.tian-w.cn

[Q07] 删除表
来源：http://awu.wangdashe.top

DROP TABLE IF EXISTS orders;
来源：http://nag.xylfe.cn

[Q08] 创建普通索引
来源：http://teb.gaohongyu789.top

CREATE INDEX idx_users_email ON users(email);
来源：http://jlg.cheryme.top

[Q09] 创建唯一索引
来源：http://dhv.aizwys.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jmp.tian-w.cn

[Q10] 插入单行
来源：http://qbl.meibo888.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hji.zhaomingkeji.xyz

[Q11] 一次插入多行
来源：http://elc.yj202588.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ioy.mhx1999.top

[Q12] 插入后取自增 ID
来源：http://ywr.fengsongda.top

INSERT INTO users (name) VALUES ('C');
来源：http://hjw.xuetiantiany.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rdd.jyoumei.cn

[Q13] 忽略重复插入
来源：http://rlm.aibaodan.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://oti.nwbrower.top

[Q14] 存在则更新（upsert）
来源：http://oqx.kuanghao11.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://aar.haohaochexian.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://him.feifeiyinyue.top

[Q15] 查询全部
来源：http://wte.ywan-chungtsiang.top

SELECT * FROM users;
来源：http://nbv.wangshuangyany.cn

[Q16] 查询指定列
来源：http://xpe.jiagoushi.top

SELECT id, name FROM users;
来源：http://dat.chenjidiqi.icu

[Q17] 条件查询
来源：http://xim.birdmap.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ajd.zhengqikj.top

[Q18] 模糊匹配
来源：http://xvd.kuanghao11.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ssp.ehwqpu.com

[Q19] 范围查询
来源：http://uqd.shanyushiyangkeji.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xff.chenlongwang.top

[Q20] IN 列表
来源：http://fnm.yfazqb.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jis.jiagoushi.top

[Q21] 空值判断
来源：http://pbe.aizwys.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://vpc.cashguo.top

[Q22] 排序
来源：http://jmp.pycfn.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://upl.shzxlz.cn

[Q23] 分页
来源：http://jfw.xylfe.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ysm.hammf.cn

[Q24] 去重
来源：http://tap.gzhubu.top

SELECT DISTINCT city FROM users;
来源：http://koq.chenjidiqi.icu

[Q25] 只取前 N 条
来源：http://pze.shanyushiyangkeji.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vch.jinyuanbaomall.cn

[Q26] 计数
来源：http://wkh.smart0.xyz

SELECT COUNT(*) FROM users;
来源：http://tqe.ybcxt.top

[Q27] 条件计数
来源：http://dtk.cashguo.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rsw.jinyuanbaomall.cn

[Q28] 求和与平均
来源：http://dwn.sxryk.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zui.iojbl.cn

[Q29] 最大最小值
来源：http://qad.zycfv.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://iqg.andypj.xyz

[Q30] 分组统计
来源：http://qew.redwolf501.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ljb.daxiang520.top

[Q31] 分组后过滤
来源：http://sgp.shanyushiyangkeji.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xqj.xingfuxueyuan.xyz

[Q32] 分组拼接字符串
来源：http://uui.ivvv.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pjz.hammf.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://yuu.jianghu66.top

[Q33] 多列分组
来源：http://lpd.smart0.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tpr.iojbl.cn

[Q34] 每组取第一条
来源：http://zzf.iojbl.cn

SELECT * FROM (
来源：http://blp.yfazqb.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wae.haohaochexian.top

) t WHERE rn = 1;
来源：http://jck.zhengqikj.top

[Q35] 内连接
来源：http://whe.yuanzhike.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tjy.dashuyun.cn

[Q36] 左连接
来源：http://qfv.hesvh.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qnc.quarkkingdee.top

[Q37] 右连接
来源：http://rdy.xinyue.icu

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nvi.yongpay.top

[Q38] 全外连接（PostgreSQL）
来源：http://std.sysykeji.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://iqk.zhiwuduotai.top

[Q39] 自连接（查上下级）
来源：http://log.yangfankeji.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://xvw.cqqwz.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wtw.andypj.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://ele.sysykeji.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pmp.chenjidiqi.icu

[Q41] 多表连接
来源：http://ulm.ybcxt.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://pgs.ivvv.top

JOIN users u ON u.id = o.user_id
来源：http://xhl.dashuyun.cn

JOIN products p ON p.id = o.product_id;
来源：http://ypb.jqgfzy.top

[Q42] 连接条件附加过滤
来源：http://uxa.pengpengdd.cyou

SELECT u.name, o.amount FROM users u
来源：http://oby.guowangkeji.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pvv.wangshuangyany.cn

[Q43] 标量子查询
来源：http://lrn.uphjek.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fvi.chenlongwang.top

[Q44] IN 子查询
来源：http://xwv.sufxvd.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://esj.hcnkem.com

[Q45] EXISTS 判断存在
来源：http://pdp.xylfe.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://svq.zhoulong.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://rgj.sweek.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bgv.shzxlz.cn

[Q47] 与平均值比较
来源：http://yrh.fzhhl.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gul.dianchejie.cn

[Q48] CTE 公用表表达式
来源：http://dfu.0kj1m.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rbk.yanxiufei.cn

SELECT * FROM t WHERE c > 5;
来源：http://phq.zhixingplan.top

[Q49] 更新单行
来源：http://glx.9152youxi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://oah.chenzaomai.com

[Q50] 批量更新
来源：http://qmc.shzxlz.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nkq.sysykeji.top

[Q51] 用子查询更新
来源：http://njl.xuetiantiany.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qqh.bbcook.cn

[Q52] 删除指定行
来源：http://gmx.zhijiandao.cn

DELETE FROM users WHERE id = 10;
来源：http://vns.fktsv.cn

[Q53] 按条件删除
来源：http://sps.fengsongda.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xlt.jianghu66.top

[Q54] 清空表
来源：http://zls.snrcjt.cn

TRUNCATE TABLE logs;
来源：http://gdp.jqgfzy.top

[Q55] 排名（并列占位）
来源：http://llx.chenzaomai.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://awk.sjlbkw.cn

[Q56] 密集排名（并列不占位）
来源：http://brs.zdqjudy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bdb.yj20258.top

[Q57] 行号
来源：http://sqp.zhoulong.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kjh.cdnleiting.top

[Q58] 累计求和
来源：http://tww.fehbvm.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xmg.jinqigfzy.top

[Q59] 分组内累计
来源：http://wdk.jinyuanbaomall.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://szp.hywenlv.cn

[Q60] 取上一行 / 下一行
来源：http://wpw.yj202588.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bnl.zhoulong.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kzo.yanxiufei.cn

[Q61] 移动平均
来源：http://ipy.yfazqb.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hnb.shangyingyoupin.top

[Q62] 分组占比
来源：http://cje.vehdjk.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bkp.yuanzhike.top

[Q63] 开启事务
来源：http://kcd.yongpay.top

START TRANSACTION;                -- 或 BEGIN
来源：http://knc.fanxiaobao.xyz

[Q64] 提交事务
来源：http://tsk.bbcook.cn

COMMIT;
来源：http://xja.guowangkeji.top

[Q65] 回滚事务
来源：http://tjk.pycfn.com

ROLLBACK;
来源：http://rdw.fzhhl.top

[Q66] 行锁查询
来源：http://coz.vqdsnc.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ttk.jinqigfzy.top

[Q67] 设置隔离级别
来源：http://dre.iojbl.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://guh.cdnleiting.top

[Q68] 保存点
来源：http://mjd.hongshengwenyu.top

SAVEPOINT sp1;
来源：http://hru.zhiwuduotai.top

ROLLBACK TO sp1;
来源：http://xtg.shzxlz.cn

[Q69] 查看执行计划
来源：http://ylt.ywan-chungtsiang.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tis.hysaishi.cn

[Q70] 更新统计信息
来源：http://cbg.kuanghao11.cn

ANALYZE TABLE users;
来源：http://kpx.yanxiufei.cn

[Q71] 查看建表语句
来源：http://ovc.nanxinkj.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pml.316326.xyz

[Q72] 查看索引
来源：http://awj.pycfn.com


<!-- 参考信息 -->
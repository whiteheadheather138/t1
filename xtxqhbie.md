代发 wailian999

================================================================================
来源：http://uam.zhengqikj.top

O. 并发与异步
来源：http://ied.shangyingyoupin.top

================================================================================
来源：http://bzw.nanxinkj.top

[O01] 启动一个线程
来源：http://eqx.daxiang520.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rzc.fanxiaobao.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://uvy.mhx1999.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pda.wangshuangyany.cn

TS:   // 同 JS
来源：http://szk.wangshuangyany.cn

Java: new Thread(() -> f()).start()
来源：http://yew.cqqwz.cn

Go:   go f()
来源：http://sgu.feifeiyinyue.top

Ruby: Thread.new { f }
来源：http://qqo.sysykeji.top

C#:   Task.Run(() => F());
来源：http://qiz.redwolf501.top

[O02] 使用线程池
来源：http://djc.zhaomingkeji.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bya.ctjpmb.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://doq.sxryk.cn

JS:   // worker_threads 线程池
来源：http://eks.vehdjk.com

TS:   // worker_threads 线程池
来源：http://vcw.tarul.cn

Java: Executors.newFixedThreadPool(4)
来源：http://lli.nwbrower.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kzl.yuxming.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fhd.jiagoushi.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xpn.zhiwuduotai.top

[O03] 加锁保护共享数据
来源：http://wlc.vqdsnc.cn

Py:   with lock: shared += 1
来源：http://erj.redwolf501.top

PHP:  // 用 flock() 做文件锁
来源：http://xdi.shzxlz.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mne.dianchejie.cn

TS:   // 同 JS
来源：http://mxw.aibaodan.cn

Java: synchronized (this) { shared++; }
来源：http://atd.guowangkeji.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qwu.jiagoushi.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://zpw.316326.xyz

C#:   lock (gate) { shared++; }
来源：http://jyv.fktsv.cn

[O04] 定义异步函数并等待
来源：http://ybh.ybcxt.top

Py:   async def f():⏎    await g()
来源：http://uwz.birdmap.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gwv.aibaodan.cn

JS:   async function f() { await g(); }
来源：http://eev.svipenyu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://qtd.yanxiufei.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mhv.sxryk.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vvr.sufxvd.cn

Ruby: # 用 Fiber 或 async gem
来源：http://jtc.daria6918.cn

C#:   async Task F() { await G(); }
来源：http://nhq.sufxvd.cn

[O05] 并发执行并等待全部完成
来源：http://wbk.yanxiufei.cn

Py:   asyncio.gather(*tasks)
来源：http://qqn.316326.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nkw.hywenlv.cn

JS:   await Promise.all(tasks)
来源：http://rlp.cdnleiting.top

TS:   await Promise.all(tasks)
来源：http://oyf.iojbl.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jaf.9152youxi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mjx.gotoacloud.top

Ruby: threads.map(&:join)
来源：http://spr.dashuyun.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ikz.hnqzz.top

[O06] 使用进程池
来源：http://ygw.hywenlv.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yff.wangdashe.top

PHP:  // pcntl_fork 或多进程队列
来源：http://xud.meibo888.top

JS:   // child_process / cluster 模块
来源：http://tij.cashguo.top

TS:   // child_process / cluster 模块
来源：http://xgu.shzxlz.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://nuu.shanyushiyangtech.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://aml.zhengqikj.top

Ruby: // fork 块
来源：http://uov.epnwcf.com

C#:   Parallel.For
来源：http://keh.vqdsnc.cn

================================================================================
来源：http://ugm.hywenlv.cn

P. 常用工具函数
来源：http://xab.cqqwz.cn

================================================================================
来源：http://dgg.sweek.top

[P01] 生成 UUID
来源：http://gnu.0kj1m.cn

Py:   str(uuid.uuid4())
来源：http://wak.xylfe.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pep.cucudq.cn

JS:   crypto.randomUUID()
来源：http://rdo.fktsv.cn

TS:   crypto.randomUUID()
来源：http://lzd.feifeiyinyue.top

Java: UUID.randomUUID().toString()
来源：http://xkd.gaohongyu789.top

Go:   // 用 github.com/google/uuid
来源：http://nnr.feifeiyinyue.top

Ruby: SecureRandom.uuid
来源：http://rgh.52xcode.cn

C#:   Guid.NewGuid().ToString()
来源：http://wln.cdnleiting.top

[P02] MD5 / SHA256 摘要
来源：http://cht.fanxiaobao.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fww.fktsv.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ilc.zhengqikj.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://way.chenlongwang.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cvi.nanxinkj.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wiz.nanxinkj.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jmn.shanyushiyangkeji.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nwa.yangfankeji.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rqy.quarkkingdee.top

[P03] 生成短随机字符串
来源：http://nrk.pycfn.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cyt.hywenlv.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ojj.c1oappe.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ffg.hnqzz.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ezw.dashuyun.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bbu.hammf.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://sqs.daxiang520.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://hml.yanxiufei.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dym.ydzc1.top

[P04] 求长度
来源：http://pet.yongpay.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ddq.xuetiantiany.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pfr.iojbl.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://krf.andypj.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hbi.hfpthk.cn

Java: list.size();  map.size();  s.length()
来源：http://kbd.iojbl.cn

Go:   len(arr);  len(m)
来源：http://mxz.jianghu66.top

Ruby: x.length;  x.size
来源：http://yth.yvedp.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ddt.yfazqb.com

[P05] 判断两个对象内容是否相等
来源：http://ftf.xziqi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://bej.shzxlz.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fev.xinyue.icu

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://uhs.guowangkeji.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://noq.fehbvm.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://oqp.hnqzz.top

Go:   reflect.DeepEqual(a, b)
来源：http://zhx.gzhubu.top

Ruby: a == b
来源：http://iim.dianchejie.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vdd.yuanzhike.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hby.xinyue.icu

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ftp.0kj1m.cn

PHP:  if (empty($x)) {}
来源：http://asb.9152youxi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://whm.hfpthk.cn

TS:   if (x == null) {}
来源：http://bpx.fengsongda.top

Java: if (x == null || x.isEmpty()) {}
来源：http://jpn.52xcode.cn

Go:   if x == nil {}
来源：http://are.pycfn.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bge.tianlin.xyz

C#:   if (x is null) {}
来源：http://xgx.xziqi.cn

[P07] 防抖与节流
来源：http://uxn.tarul.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zbt.aizwys.cn

PHP:  // 手写时间戳比较
来源：http://jpp.jqgfzy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://slz.iojbl.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jjg.ywan-chungtsiang.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://oov.zycfv.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lvf.hnqzz.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://wwe.svipenyu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fgn.yfazqb.com

[P08] 处理浮点精度问题
来源：http://col.cucudq.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kdu.daria6918.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://tqj.yfazqb.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xki.cqqwz.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://iko.aibaodan.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dhn.cdnleiting.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ljv.zhengqikj.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qyr.cashguo.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://srm.guowangkeji.top

================================================================================
来源：http://mlk.zdqjudy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wmg.cheryme.top

================================================================================
来源：http://wyo.52xcode.cn

[Q01] 创建表
来源：http://eun.birdmap.top

CREATE TABLE users (
来源：http://bll.gaohongyu789.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hnm.dashuyun.cn

name VARCHAR(50) NOT NULL,
来源：http://mhf.xinyue.icu

email VARCHAR(100) UNIQUE,
来源：http://tpi.gotoacloud.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zbo.ywan-chungtsiang.top

);
来源：http://okk.cheryme.top

[Q02] 创建带外键的表
来源：http://ssl.tanke756.top

CREATE TABLE orders (
来源：http://dro.zhaomingkeji.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jze.epnwcf.com

user_id INT NOT NULL,
来源：http://hdt.daria6918.cn

amount DECIMAL(10, 2),
来源：http://yzz.jinyuanbaomall.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rrg.zhaomingkeji.xyz

);
来源：http://fjd.hongshengwenyu.top

[Q03] 增加列
来源：http://wsk.ivvv.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jfp.yuanzhike.top

[Q04] 修改列类型
来源：http://zwq.shanyushiyangtech.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fcj.quarkkingdee.top

[Q05] 重命名列
来源：http://upb.kuanghao11.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bxf.hywenlv.cn

[Q06] 删除列
来源：http://hqw.ybcxt.top

ALTER TABLE users DROP COLUMN age;
来源：http://zrw.fzhhl.top

[Q07] 删除表
来源：http://xld.ppjwa.cn

DROP TABLE IF EXISTS orders;
来源：http://fxf.yuxming.cn

[Q08] 创建普通索引
来源：http://rll.hfpthk.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://vsx.jinghuilouyu.cn

[Q09] 创建唯一索引
来源：http://wmb.hywenlv.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xzk.nanxinkj.top

[Q10] 插入单行
来源：http://xrx.yj20258.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jmk.epnwcf.com

[Q11] 一次插入多行
来源：http://fkw.ydjk.org.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lvp.zhiwuduotai.top

[Q12] 插入后取自增 ID
来源：http://vkw.tian-w.cn

INSERT INTO users (name) VALUES ('C');
来源：http://uqe.sweek.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jps.ehwqpu.com

[Q13] 忽略重复插入
来源：http://gcs.xingfuxueyuan.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://sbh.quarkkingdee.top

[Q14] 存在则更新（upsert）
来源：http://jwm.vehdjk.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wxk.0kj1m.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ubr.dashuyun.cn

[Q15] 查询全部
来源：http://isi.yonumen.top

SELECT * FROM users;
来源：http://hqg.daria6918.cn

[Q16] 查询指定列
来源：http://aoi.hcnkem.com

SELECT id, name FROM users;
来源：http://siu.vehdjk.com

[Q17] 条件查询
来源：http://ije.gzhubu.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://crd.zycfv.cn

[Q18] 模糊匹配
来源：http://ini.xylfe.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zbv.cdnleiting.top

[Q19] 范围查询
来源：http://jse.havefunace.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ydt.0kj1m.cn

[Q20] IN 列表
来源：http://nsy.sufxvd.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://oqz.wangshuangyany.cn

[Q21] 空值判断
来源：http://qrx.birdmap.top

SELECT * FROM users WHERE email IS NULL;
来源：http://lux.aibaodan.cn

[Q22] 排序
来源：http://bxi.zhijiandao.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nzj.nwbrower.top

[Q23] 分页
来源：http://cvo.jiagoushi.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://srp.yueranfly.top

[Q24] 去重
来源：http://hbo.yanxiufei.cn

SELECT DISTINCT city FROM users;
来源：http://vvd.pycfn.com

[Q25] 只取前 N 条
来源：http://trk.quarkkingdee.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lzd.sjlbkw.cn

[Q26] 计数
来源：http://xzj.daria6918.cn

SELECT COUNT(*) FROM users;
来源：http://wks.0kj1m.cn

[Q27] 条件计数
来源：http://qcv.zhixingplan.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fwk.316326.xyz

[Q28] 求和与平均
来源：http://ydq.xuetiantiany.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://oby.0kj1m.cn

[Q29] 最大最小值
来源：http://ljv.hammf.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://itv.tianlin.xyz

[Q30] 分组统计
来源：http://hwj.yfazqb.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cbd.xziqi.cn

[Q31] 分组后过滤
来源：http://tad.iojbl.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wry.ctjpmb.com

[Q32] 分组拼接字符串
来源：http://whc.vehdjk.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://oqj.chenjidiqi.icu

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lai.xinyue.icu

[Q33] 多列分组
来源：http://gof.cheryme.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gij.xinyue.icu

[Q34] 每组取第一条
来源：http://uaf.yuxming.cn

SELECT * FROM (
来源：http://dpg.hammf.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://uyj.jianghu66.top

) t WHERE rn = 1;
来源：http://eql.xinyue.icu

[Q35] 内连接
来源：http://suz.jinqigfzy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hav.chenlongwang.top

[Q36] 左连接
来源：http://emg.smart0.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://esz.0kj1m.cn

[Q37] 右连接
来源：http://cdj.fehbvm.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hhp.gzhubu.top

[Q38] 全外连接（PostgreSQL）
来源：http://hpv.iojbl.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kbi.ctjpmb.com

[Q39] 自连接（查上下级）
来源：http://hca.yongpay.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://xnf.ctjpmb.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wub.fanxiaobao.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://vcb.cheryme.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pib.yuanzhike.top

[Q41] 多表连接
来源：http://pws.fzhhl.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://mtt.chenzaomai.com

JOIN users u ON u.id = o.user_id
来源：http://yjl.mhx1999.top

JOIN products p ON p.id = o.product_id;
来源：http://wwg.hesvh.cn

[Q42] 连接条件附加过滤
来源：http://oiq.sweek.top

SELECT u.name, o.amount FROM users u
来源：http://jsz.zhoulong.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zgu.sweek.top

[Q43] 标量子查询
来源：http://cuq.havefunace.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://isq.cqqwz.cn

[Q44] IN 子查询
来源：http://lpu.yuanzhike.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ufx.kuanghao11.cn

[Q45] EXISTS 判断存在
来源：http://pwr.sysykeji.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fwd.kuanghao11.cn

[Q46] NOT EXISTS 判断不存在
来源：http://qwn.pycfn.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uhx.c1oappe.top

[Q47] 与平均值比较
来源：http://zng.daxiang520.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qkm.shzxlz.cn

[Q48] CTE 公用表表达式
来源：http://csp.zhoulong.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://etb.0kj1m.cn

SELECT * FROM t WHERE c > 5;
来源：http://bcl.yvedp.cn

[Q49] 更新单行
来源：http://itb.cashguo.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fmy.pengpengdd.cyou

[Q50] 批量更新
来源：http://foe.ctjpmb.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://esb.daxiang520.top

[Q51] 用子查询更新
来源：http://qsh.wangshuangyany.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ryo.hywenlv.cn

[Q52] 删除指定行
来源：http://hjb.shanyushiyangtech.top

DELETE FROM users WHERE id = 10;
来源：http://dys.yj20258.top

[Q53] 按条件删除
来源：http://ftp.zdbjq.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vbj.jianghu66.top

[Q54] 清空表
来源：http://btc.xziqi.cn

TRUNCATE TABLE logs;
来源：http://ztz.fktsv.cn

[Q55] 排名（并列占位）
来源：http://izy.tian-w.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bdd.xziqi.cn

[Q56] 密集排名（并列不占位）
来源：http://atj.guannengcc.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yml.shanyushiyangkeji.top

[Q57] 行号
来源：http://qna.daria6918.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ndo.jinqigufen.top

[Q58] 累计求和
来源：http://lll.aibaodan.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://icd.ywan-chungtsiang.top

[Q59] 分组内累计
来源：http://zox.tian-w.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://clv.yanxiufei.cn

[Q60] 取上一行 / 下一行
来源：http://prn.yuanzhike.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cfo.iojbl.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kzm.chenzaomai.com

[Q61] 移动平均
来源：http://cxm.fzhhl.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jia.yangfankeji.com

[Q62] 分组占比
来源：http://ags.yj20258.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wqp.xinyue.icu

[Q63] 开启事务
来源：http://haj.guowangkeji.top

START TRANSACTION;                -- 或 BEGIN
来源：http://bht.tanke756.top

[Q64] 提交事务
来源：http://skn.yongpay.top

COMMIT;
来源：http://dnw.aizwys.cn

[Q65] 回滚事务
来源：http://ysq.ivvv.top

ROLLBACK;
来源：http://ahn.pycfn.com

[Q66] 行锁查询
来源：http://izv.yj20258.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://krp.gzhubu.top

[Q67] 设置隔离级别
来源：http://duh.guowangkeji.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lfn.xingfuxueyuan.xyz

[Q68] 保存点
来源：http://xrp.zhijiandao.cn

SAVEPOINT sp1;
来源：http://iwr.xuanzx.com

ROLLBACK TO sp1;
来源：http://ata.jinqigfzy.top

[Q69] 查看执行计划
来源：http://hgy.shzxlz.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dns.jinyuanbaomall.cn

[Q70] 更新统计信息
来源：http://cof.yanxiufei.cn

ANALYZE TABLE users;
来源：http://czf.wangshuangyany.cn

[Q71] 查看建表语句
来源：http://mdl.feifeiyinyue.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wcl.ctjpmb.com

[Q72] 查看索引
来源：http://ejq.guannengcc.top


<!-- 参考信息 -->
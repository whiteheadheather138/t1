代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rag.jinghuilouyu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ylw.bbcook.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pai.ivvv.top

TS:   // 同 JS
来源：http://mpm.gogol.net.cn

Java: new Thread(() -> f()).start()
来源：http://pjg.sysykeji.top

Go:   go f()
来源：http://kwl.kuanghao11.cn

Ruby: Thread.new { f }
来源：http://vlf.shzxlz.cn

C#:   Task.Run(() => F());
来源：http://jgj.yonumen.top

[O02] 使用线程池
来源：http://glp.hywenlv.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gfa.hcnkem.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wru.sufxvd.cn

JS:   // worker_threads 线程池
来源：http://vmd.ybcxt.top

TS:   // worker_threads 线程池
来源：http://uoo.xuetiantiany.cn

Java: Executors.newFixedThreadPool(4)
来源：http://oek.uphjek.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://czq.fengsongda.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cmj.zhiwuduotai.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gax.jlsjyb.cn

[O03] 加锁保护共享数据
来源：http://kkp.yvedp.cn

Py:   with lock: shared += 1
来源：http://oax.chenlongwang.top

PHP:  // 用 flock() 做文件锁
来源：http://buj.xuetiantiany.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://epm.mhx1999.top

TS:   // 同 JS
来源：http://ayv.jinqigufen.top

Java: synchronized (this) { shared++; }
来源：http://bee.52xcode.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://whq.quarkkingdee.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://gdw.cdnleiting.top

C#:   lock (gate) { shared++; }
来源：http://vml.zhaomingkeji.xyz

[O04] 定义异步函数并等待
来源：http://aee.tian-w.cn

Py:   async def f():⏎    await g()
来源：http://dne.guowangkeji.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lvj.nanxinkj.top

JS:   async function f() { await g(); }
来源：http://eug.chenzaomai.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://ric.dashuyun.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hel.zhaomingkeji.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vwx.yj20258.top

Ruby: # 用 Fiber 或 async gem
来源：http://gxs.nanxinkj.top

C#:   async Task F() { await G(); }
来源：http://sry.jyoumei.cn

[O05] 并发执行并等待全部完成
来源：http://fig.ehwqpu.com

Py:   asyncio.gather(*tasks)
来源：http://bto.haohaochexian.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tcg.nanxinkj.top

JS:   await Promise.all(tasks)
来源：http://jbx.shuidangran.top

TS:   await Promise.all(tasks)
来源：http://rfh.hnxiangtu.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pdz.yuanzhike.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mxt.c1oappe.top

Ruby: threads.map(&:join)
来源：http://ufx.wangdashe.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ebh.gzhubu.top

[O06] 使用进程池
来源：http://mjy.yonumen.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lvq.shuidangran.top

PHP:  // pcntl_fork 或多进程队列
来源：http://knf.fktsv.cn

JS:   // child_process / cluster 模块
来源：http://hya.c1oappe.top

TS:   // child_process / cluster 模块
来源：http://xer.zhoulong.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://eyj.mhx1999.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ubl.hesvh.cn

Ruby: // fork 块
来源：http://uab.ybcxt.top

C#:   Parallel.For
来源：http://dlg.zhongyouzk.top

================================================================================
来源：http://meu.chenzaomai.com

P. 常用工具函数
来源：http://luv.tarul.cn

================================================================================
来源：http://ubs.vehdjk.com

[P01] 生成 UUID
来源：http://ugj.ivvv.top

Py:   str(uuid.uuid4())
来源：http://qob.sufxvd.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ovz.316326.xyz

JS:   crypto.randomUUID()
来源：http://xsn.zhongyouzk.top

TS:   crypto.randomUUID()
来源：http://poi.jiagoushi.top

Java: UUID.randomUUID().toString()
来源：http://ggd.redwolf501.top

Go:   // 用 github.com/google/uuid
来源：http://iyp.hywenlv.cn

Ruby: SecureRandom.uuid
来源：http://euj.yangfankeji.com

C#:   Guid.NewGuid().ToString()
来源：http://iww.bjfxy.top

[P02] MD5 / SHA256 摘要
来源：http://hvz.hammf.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rur.jinqigufen.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://nvr.nanxinkj.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ppi.gaohongyu789.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ccl.hesvh.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cac.yonumen.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ghy.yueranfly.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ncm.daxiang520.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://shv.redwolf501.top

[P03] 生成短随机字符串
来源：http://bkr.redwolf501.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pog.xuanzx.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kun.jlsjyb.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://awh.cheryme.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://awq.zhijiandao.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zwl.dashuyun.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://uye.0kj1m.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://oqn.hnxiangtu.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mlu.zhongyouzk.top

[P04] 求长度
来源：http://wbb.zhiwuduotai.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gno.fzhhl.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pao.sxryk.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ruc.guowangkeji.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ynu.pycfn.com

Java: list.size();  map.size();  s.length()
来源：http://fzy.uphjek.com

Go:   len(arr);  len(m)
来源：http://mbq.dianchejie.cn

Ruby: x.length;  x.size
来源：http://wbm.smart0.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://tgh.9152youxi.cn

[P05] 判断两个对象内容是否相等
来源：http://gok.xziqi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://glr.hywenlv.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qks.kuanghao11.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qqv.zhongyouzk.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://pje.vehdjk.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xyi.zhoulong.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://vfx.haohaochexian.top

Ruby: a == b
来源：http://ldj.yongpay.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://onl.hnqzz.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kvg.andypj.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yjq.cashguo.top

PHP:  if (empty($x)) {}
来源：http://etn.hnqzz.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hjl.yanxiufei.cn

TS:   if (x == null) {}
来源：http://uzf.chenjidiqi.icu

Java: if (x == null || x.isEmpty()) {}
来源：http://sch.nanxuanxn.top

Go:   if x == nil {}
来源：http://raw.sufxvd.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vfd.sysykeji.top

C#:   if (x is null) {}
来源：http://zpu.yuxming.cn

[P07] 防抖与节流
来源：http://rfs.xinyue.icu

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://eto.yonumen.top

PHP:  // 手写时间戳比较
来源：http://ara.uphjek.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cdg.iojbl.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yic.jinqigfzy.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jzl.zycfv.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://idg.hywenlv.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://xmd.yonumen.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mlw.feifeiyinyue.top

[P08] 处理浮点精度问题
来源：http://lck.jqgfzy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wze.316326.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xqu.chenzaomai.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zxx.ywan-chungtsiang.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://sso.yfazqb.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://muf.hammf.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cfw.ydjk.org.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ylq.shzxlz.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vvh.shzxlz.cn

================================================================================
来源：http://jro.shanyushiyangtech.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fuq.shanyushiyangtech.top

================================================================================
来源：http://idm.c1oappe.top

[Q01] 创建表
来源：http://sjo.316326.xyz

CREATE TABLE users (
来源：http://ykz.tanke756.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bjh.hnqzz.top

name VARCHAR(50) NOT NULL,
来源：http://hcf.snrcjt.cn

email VARCHAR(100) UNIQUE,
来源：http://jhm.ywan-chungtsiang.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://eoe.zhoulong.xyz

);
来源：http://kwr.zdqjudy.top

[Q02] 创建带外键的表
来源：http://rdn.ehwqpu.com

CREATE TABLE orders (
来源：http://oej.birdmap.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wiy.dianchejie.cn

user_id INT NOT NULL,
来源：http://wbg.xinyue.icu

amount DECIMAL(10, 2),
来源：http://hvq.ywan-chungtsiang.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ked.52xcode.cn

);
来源：http://ehp.zhengqikj.top

[Q03] 增加列
来源：http://pvu.havefunace.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dcq.uphjek.com

[Q04] 修改列类型
来源：http://obo.zhaomingkeji.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://chs.jyoumei.cn

[Q05] 重命名列
来源：http://rkh.9152youxi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ekv.hnqzz.top

[Q06] 删除列
来源：http://rbc.epnwcf.com

ALTER TABLE users DROP COLUMN age;
来源：http://hve.aizwys.cn

[Q07] 删除表
来源：http://pij.tianlin.xyz

DROP TABLE IF EXISTS orders;
来源：http://vem.xuanzx.com

[Q08] 创建普通索引
来源：http://qkb.ctjpmb.com

CREATE INDEX idx_users_email ON users(email);
来源：http://rtd.cucudq.cn

[Q09] 创建唯一索引
来源：http://teo.wangshuangyany.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yhh.ehwqpu.com

[Q10] 插入单行
来源：http://guo.bbcook.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://obe.shangyingyoupin.top

[Q11] 一次插入多行
来源：http://cmu.hnqzz.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vqe.zhoulong.xyz

[Q12] 插入后取自增 ID
来源：http://gyn.yongpay.top

INSERT INTO users (name) VALUES ('C');
来源：http://jhr.yangfankeji.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mmy.xylfe.cn

[Q13] 忽略重复插入
来源：http://odf.shzxlz.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kba.chenzaomai.com

[Q14] 存在则更新（upsert）
来源：http://szc.feifeiyinyue.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ygi.52xcode.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mwg.mhx1999.top

[Q15] 查询全部
来源：http://qeq.sweek.top

SELECT * FROM users;
来源：http://lyc.smart0.xyz

[Q16] 查询指定列
来源：http://kmt.aizwys.cn

SELECT id, name FROM users;
来源：http://kqs.ehwqpu.com

[Q17] 条件查询
来源：http://skj.daxiang520.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://grl.yj20258888.top

[Q18] 模糊匹配
来源：http://zhh.tian-w.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mza.guowangkeji.top

[Q19] 范围查询
来源：http://dox.fengsongda.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jcb.yanxiufei.cn

[Q20] IN 列表
来源：http://ydr.0kj1m.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lhe.guowangkeji.top

[Q21] 空值判断
来源：http://ndw.ydjk.org.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://gbe.smart0.xyz

[Q22] 排序
来源：http://yix.c1oappe.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mms.shanyushiyangtech.top

[Q23] 分页
来源：http://yka.hammf.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ube.xinyue.icu

[Q24] 去重
来源：http://krx.hywenlv.cn

SELECT DISTINCT city FROM users;
来源：http://vpe.pengpengdd.cyou

[Q25] 只取前 N 条
来源：http://dkm.dianchejie.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nce.fzhhl.top

[Q26] 计数
来源：http://wdw.cucudq.cn

SELECT COUNT(*) FROM users;
来源：http://air.shangyingyoupin.top

[Q27] 条件计数
来源：http://vri.mhx1999.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mci.iojbl.cn

[Q28] 求和与平均
来源：http://kbl.0kj1m.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://doy.ydzc1.top

[Q29] 最大最小值
来源：http://xfa.zdbjq.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://yll.ybcxt.top

[Q30] 分组统计
来源：http://llo.daxiang520.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nwi.zhixingplan.top

[Q31] 分组后过滤
来源：http://hld.fktsv.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bsk.xingfuxueyuan.xyz

[Q32] 分组拼接字符串
来源：http://nog.jiagoushi.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hzd.yuxming.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://aun.nanxinkj.top

[Q33] 多列分组
来源：http://efp.jinqigufen.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tfd.bbcook.cn

[Q34] 每组取第一条
来源：http://xbf.xinyue.icu

SELECT * FROM (
来源：http://kbp.hnqzz.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rwh.jlsjyb.cn

) t WHERE rn = 1;
来源：http://hvl.hnxiangtu.top

[Q35] 内连接
来源：http://drj.ivvv.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bil.cashguo.top

[Q36] 左连接
来源：http://ssr.ivvv.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hrj.yangfankeji.com

[Q37] 右连接
来源：http://ilx.hfpthk.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kbc.chenzaomai.com

[Q38] 全外连接（PostgreSQL）
来源：http://cdi.jyoumei.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hie.yj20258888.top

[Q39] 自连接（查上下级）
来源：http://cyj.jinyuanbaomall.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://nsh.yongpay.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wkd.xziqi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://nyf.yvedp.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hmh.cdnleiting.top

[Q41] 多表连接
来源：http://ppj.yj20258.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://tzt.52xcode.cn

JOIN users u ON u.id = o.user_id
来源：http://zsh.cashguo.top

JOIN products p ON p.id = o.product_id;
来源：http://oai.zhixingplan.top

[Q42] 连接条件附加过滤
来源：http://gkk.shanyushiyangtech.top

SELECT u.name, o.amount FROM users u
来源：http://nan.quarkkingdee.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xza.zhiwuduotai.top

[Q43] 标量子查询
来源：http://fww.snrcjt.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gyl.316326.xyz

[Q44] IN 子查询
来源：http://bpx.sxryk.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ivi.0kj1m.cn

[Q45] EXISTS 判断存在
来源：http://nvm.jinqigfzy.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wve.shzxlz.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xbe.52xcode.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jet.tian-w.cn

[Q47] 与平均值比较
来源：http://wyd.vehdjk.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rci.tianlin.xyz

[Q48] CTE 公用表表达式
来源：http://xwx.shangyingyoupin.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qwq.nanxinkj.top

SELECT * FROM t WHERE c > 5;
来源：http://mrg.cdnleiting.top

[Q49] 更新单行
来源：http://wnu.gotoacloud.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dwy.tanke756.top

[Q50] 批量更新
来源：http://qef.vehdjk.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jkm.ywan-chungtsiang.top

[Q51] 用子查询更新
来源：http://tdo.zhiwuduotai.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dop.mhx1999.top

[Q52] 删除指定行
来源：http://trp.wangdashe.top

DELETE FROM users WHERE id = 10;
来源：http://lvm.ppjwa.cn

[Q53] 按条件删除
来源：http://hln.cheryme.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bcu.tanke756.top

[Q54] 清空表
来源：http://aam.hnxiangtu.top

TRUNCATE TABLE logs;
来源：http://yje.tianlin.xyz

[Q55] 排名（并列占位）
来源：http://wqw.shanyushiyangtech.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kwd.ctjpmb.com

[Q56] 密集排名（并列不占位）
来源：http://wjl.hfpthk.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://swt.xingfuxueyuan.xyz

[Q57] 行号
来源：http://uwk.fehbvm.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gdy.haohaochexian.top

[Q58] 累计求和
来源：http://bdz.ivvv.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ssm.uphjek.com

[Q59] 分组内累计
来源：http://rkm.jqgfzy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://eyo.gzhubu.top

[Q60] 取上一行 / 下一行
来源：http://uch.zhaomingkeji.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ptg.epnwcf.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fcs.quarkkingdee.top

[Q61] 移动平均
来源：http://fyq.xingfuxueyuan.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://uip.daria6918.cn

[Q62] 分组占比
来源：http://uqw.nanxinkj.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hin.tian-w.cn

[Q63] 开启事务
来源：http://tqy.hnqzz.top

START TRANSACTION;                -- 或 BEGIN
来源：http://gee.fengsongda.top

[Q64] 提交事务
来源：http://uhm.ppjwa.cn

COMMIT;
来源：http://nhm.yj202588.top

[Q65] 回滚事务
来源：http://hsy.jianghu66.top

ROLLBACK;
来源：http://vcq.daxiang520.top

[Q66] 行锁查询
来源：http://qif.zhiwuduotai.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rzo.hnqzz.top

[Q67] 设置隔离级别
来源：http://zhq.ybcxt.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wmm.birdmap.top

[Q68] 保存点
来源：http://idc.yanxiufei.cn

SAVEPOINT sp1;
来源：http://pbx.nanxuanxn.top

ROLLBACK TO sp1;
来源：http://nog.nanxinkj.top

[Q69] 查看执行计划
来源：http://iwk.cashguo.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yrv.nanxinkj.top

[Q70] 更新统计信息
来源：http://qux.cucudq.cn

ANALYZE TABLE users;
来源：http://las.jianghu66.top

[Q71] 查看建表语句
来源：http://yot.ydzc1.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jxd.shanyushiyangtech.top

[Q72] 查看索引
来源：http://lbg.svipenyu.cn

SHOW INDEX FROM users;
来源：http://kuu.hfpthk.cn

[Q73] 查看表状态
来源：http://hoe.ctjpmb.com

SHOW TABLE STATUS LIKE 'users';
来源：http://poc.zhaomingkeji.xyz

[Q74] 强制使用索引
来源：http://xlq.gaohongyu789.top


<!-- 参考信息 -->
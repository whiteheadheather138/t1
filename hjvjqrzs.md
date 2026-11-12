代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wkn.kuanghao11.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://len.hysaishi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uas.pengpengdd.cyou

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rwv.zhengqikj.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yvm.nanxuanxn.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dja.zycfv.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ryf.9152youxi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mki.yj20258.top

================================================================================
来源：http://gty.ivvv.top

O. 并发与异步
来源：http://vnf.zhiwuduotai.top

================================================================================
来源：http://erq.jqgfzy.top

[O01] 启动一个线程
来源：http://hxz.yonumen.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ovi.snrcjt.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ckl.cqqwz.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wpg.cdnleiting.top

TS:   // 同 JS
来源：http://czx.uphjek.com

Java: new Thread(() -> f()).start()
来源：http://upd.jlsjyb.cn

Go:   go f()
来源：http://dog.wangdashe.top

Ruby: Thread.new { f }
来源：http://wbl.zdqjudy.top

C#:   Task.Run(() => F());
来源：http://rcj.zycfv.cn

[O02] 使用线程池
来源：http://vje.yanxiufei.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bld.zhixingplan.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tua.hysaishi.cn

JS:   // worker_threads 线程池
来源：http://yzx.aibaodan.cn

TS:   // worker_threads 线程池
来源：http://bnj.0kj1m.cn

Java: Executors.newFixedThreadPool(4)
来源：http://gqd.chenlongwang.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://iog.jiagoushi.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jvh.jinghuilouyu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hhf.yongpay.top

[O03] 加锁保护共享数据
来源：http://izs.ppjwa.cn

Py:   with lock: shared += 1
来源：http://xzm.zhixingplan.top

PHP:  // 用 flock() 做文件锁
来源：http://llo.fengsongda.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://deb.sxryk.cn

TS:   // 同 JS
来源：http://gbn.ctjpmb.com

Java: synchronized (this) { shared++; }
来源：http://gyw.pycfn.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rgy.gotoacloud.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://wnp.redwolf501.top

C#:   lock (gate) { shared++; }
来源：http://hfp.52xcode.cn

[O04] 定义异步函数并等待
来源：http://kcm.ydjk.org.cn

Py:   async def f():⏎    await g()
来源：http://lxr.yj20258888.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rbz.fanxiaobao.xyz

JS:   async function f() { await g(); }
来源：http://gtx.vqdsnc.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://yse.dashuyun.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nas.tanke756.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jmw.zdbjq.cn

Ruby: # 用 Fiber 或 async gem
来源：http://dij.yongpay.top

C#:   async Task F() { await G(); }
来源：http://fnu.pengpengdd.cyou

[O05] 并发执行并等待全部完成
来源：http://jft.chenlongwang.top

Py:   asyncio.gather(*tasks)
来源：http://zpr.ehwqpu.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qhg.yvedp.cn

JS:   await Promise.all(tasks)
来源：http://qsm.shuidangran.top

TS:   await Promise.all(tasks)
来源：http://qvy.shanyushiyangtech.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bgz.chenlongwang.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://exz.chenlongwang.top

Ruby: threads.map(&:join)
来源：http://pfs.zhongyouzk.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ego.jiagoushi.top

[O06] 使用进程池
来源：http://pyx.ydjk.org.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pqg.dianchejie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://pam.ywan-chungtsiang.top

JS:   // child_process / cluster 模块
来源：http://inf.zdqjudy.top

TS:   // child_process / cluster 模块
来源：http://vbb.jiagoushi.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://euf.xuetiantiany.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://udz.vqdsnc.cn

Ruby: // fork 块
来源：http://iyu.ydzc1.top

C#:   Parallel.For
来源：http://pjl.dianchejie.cn

================================================================================
来源：http://ouv.zycfv.cn

P. 常用工具函数
来源：http://mks.epnwcf.com

================================================================================
来源：http://hrt.ehwqpu.com

[P01] 生成 UUID
来源：http://cnp.kuanghao11.cn

Py:   str(uuid.uuid4())
来源：http://vrs.sysykeji.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lvz.jqgfzy.top

JS:   crypto.randomUUID()
来源：http://vjr.cdnleiting.top

TS:   crypto.randomUUID()
来源：http://cko.shanyushiyangkeji.top

Java: UUID.randomUUID().toString()
来源：http://ugt.gogol.net.cn

Go:   // 用 github.com/google/uuid
来源：http://pgo.zhixingplan.top

Ruby: SecureRandom.uuid
来源：http://iuq.zhengqikj.top

C#:   Guid.NewGuid().ToString()
来源：http://wqb.zhongyouzk.top

[P02] MD5 / SHA256 摘要
来源：http://kop.zdbjq.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dog.chenzaomai.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://gko.c1oappe.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lxp.hysaishi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nmp.aizwys.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qgk.hongshengwenyu.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cbn.hfpthk.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gwj.jqgufenzy.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sia.xylfe.cn

[P03] 生成短随机字符串
来源：http://ggf.aibaodan.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xtq.cdnleiting.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hxm.zdbjq.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rto.dashuyun.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://phx.shzxlz.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cje.fengsongda.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://doz.chenzaomai.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://dks.wangshuangyany.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wlt.haohaochexian.top

[P04] 求长度
来源：http://vxj.fktsv.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ggp.ybcxt.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kcr.hammf.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://luo.yj202588.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dlz.jyoumei.cn

Java: list.size();  map.size();  s.length()
来源：http://uet.guannengcc.top

Go:   len(arr);  len(m)
来源：http://ord.zhaomingkeji.xyz

Ruby: x.length;  x.size
来源：http://zha.mhx1999.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://olh.nanxinkj.top

[P05] 判断两个对象内容是否相等
来源：http://csg.chenjidiqi.icu

Py:   a == b              # 列表与字典递归比较内容
来源：http://uok.jiagoushi.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://oen.jinghuilouyu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://edn.sufxvd.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hiu.jiagoushi.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ujj.xylfe.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ert.wangdashe.top

Ruby: a == b
来源：http://ptw.xingfuxueyuan.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vgs.smart0.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bpc.dashuyun.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dpf.shanyushiyangtech.top

PHP:  if (empty($x)) {}
来源：http://bic.dashuyun.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pjk.fktsv.cn

TS:   if (x == null) {}
来源：http://djl.andypj.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://qib.hcnkem.com

Go:   if x == nil {}
来源：http://bbs.ydjk.org.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mkz.xinyue.icu

C#:   if (x is null) {}
来源：http://fun.sufxvd.cn

[P07] 防抖与节流
来源：http://rtc.birdmap.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://feu.guannengcc.top

PHP:  // 手写时间戳比较
来源：http://xsp.aibaodan.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://azt.yj20258.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://all.zycfv.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://azc.yonumen.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ppr.jinghuilouyu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://hmb.yangfankeji.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://trb.sufxvd.cn

[P08] 处理浮点精度问题
来源：http://keh.mhx1999.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hdm.fengsongda.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ogr.cdnleiting.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cpd.hesvh.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hby.chenjidiqi.icu

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rxy.chenjidiqi.icu

Go:   math/big.Float，或全部换算成整数分再算
来源：http://din.fktsv.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ljn.dashuyun.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nkh.pycfn.com

================================================================================
来源：http://ttv.tian-w.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mtm.dashuyun.cn

================================================================================
来源：http://pdy.kuanghao11.cn

[Q01] 创建表
来源：http://fow.hysaishi.cn

CREATE TABLE users (
来源：http://wip.jlsjyb.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://suq.wangshuangyany.cn

name VARCHAR(50) NOT NULL,
来源：http://sep.zhengqikj.top

email VARCHAR(100) UNIQUE,
来源：http://abz.chenzaomai.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kwd.yuxming.cn

);
来源：http://pes.redwolf501.top

[Q02] 创建带外键的表
来源：http://fvq.bjfxy.top

CREATE TABLE orders (
来源：http://gmm.shzxlz.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bfx.jinyuanbaomall.cn

user_id INT NOT NULL,
来源：http://ryb.daria6918.cn

amount DECIMAL(10, 2),
来源：http://mjk.zdbjq.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zgc.ppjwa.cn

);
来源：http://flw.andypj.xyz

[Q03] 增加列
来源：http://jix.sxryk.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kbq.aizwys.cn

[Q04] 修改列类型
来源：http://dxu.fktsv.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yqw.zhongyouzk.top

[Q05] 重命名列
来源：http://yyu.vehdjk.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hmh.bjfxy.top

[Q06] 删除列
来源：http://wwt.jqgfzy.top

ALTER TABLE users DROP COLUMN age;
来源：http://uma.redwolf501.top

[Q07] 删除表
来源：http://ufr.ehwqpu.com

DROP TABLE IF EXISTS orders;
来源：http://iho.zdqjudy.top

[Q08] 创建普通索引
来源：http://jgv.sweek.top

CREATE INDEX idx_users_email ON users(email);
来源：http://xaw.ehwqpu.com

[Q09] 创建唯一索引
来源：http://sfc.daria6918.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://glr.yuanzhike.top

[Q10] 插入单行
来源：http://inj.ctjpmb.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kmb.dashuyun.cn

[Q11] 一次插入多行
来源：http://gql.gotoacloud.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://afh.zycfv.cn

[Q12] 插入后取自增 ID
来源：http://soc.chenzaomai.com

INSERT INTO users (name) VALUES ('C');
来源：http://gfd.vehdjk.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dau.tanke756.top

[Q13] 忽略重复插入
来源：http://wgc.zhiwuduotai.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fon.zhaomingkeji.xyz

[Q14] 存在则更新（upsert）
来源：http://fzy.svipenyu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rlf.xingfuxueyuan.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kod.epnwcf.com

[Q15] 查询全部
来源：http://ewt.cheryme.top

SELECT * FROM users;
来源：http://tyg.tian-w.cn

[Q16] 查询指定列
来源：http://toh.yj20258888.top

SELECT id, name FROM users;
来源：http://yij.birdmap.top

[Q17] 条件查询
来源：http://lma.52xcode.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hyz.ydzc1.top

[Q18] 模糊匹配
来源：http://tin.hammf.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hxv.jinyuanbaomall.cn

[Q19] 范围查询
来源：http://qix.daria6918.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yvl.xinyue.icu

[Q20] IN 列表
来源：http://qbh.jinqigfzy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vrk.andypj.xyz

[Q21] 空值判断
来源：http://bvq.haohaochexian.top

SELECT * FROM users WHERE email IS NULL;
来源：http://gll.cdnleiting.top

[Q22] 排序
来源：http://kww.wangdashe.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://umq.hysaishi.cn

[Q23] 分页
来源：http://kdv.daxiang520.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://erq.ehwqpu.com

[Q24] 去重
来源：http://tzz.ydzc1.top

SELECT DISTINCT city FROM users;
来源：http://mrj.birdmap.top

[Q25] 只取前 N 条
来源：http://sbc.xuanzx.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ema.dashuyun.cn

[Q26] 计数
来源：http://rxz.birdmap.top

SELECT COUNT(*) FROM users;
来源：http://jsv.9152youxi.cn

[Q27] 条件计数
来源：http://yqc.tanke756.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wnz.sufxvd.cn

[Q28] 求和与平均
来源：http://whk.guannengcc.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lyf.jianghu66.top

[Q29] 最大最小值
来源：http://tum.52xcode.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ctv.chenjidiqi.icu

[Q30] 分组统计
来源：http://pch.sysykeji.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://sbd.cashguo.top

[Q31] 分组后过滤
来源：http://egk.sjlbkw.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zis.meibo888.top

[Q32] 分组拼接字符串
来源：http://kxn.yueranfly.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://plk.haohaochexian.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ccp.hcnkem.com

[Q33] 多列分组
来源：http://jti.zhiwuduotai.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gcg.yueranfly.top

[Q34] 每组取第一条
来源：http://pej.zdbjq.cn

SELECT * FROM (
来源：http://bjg.xuanzx.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zvz.cdnleiting.top

) t WHERE rn = 1;
来源：http://nhw.yongpay.top

[Q35] 内连接
来源：http://fss.tarul.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xkj.cheryme.top

[Q36] 左连接
来源：http://veu.jyoumei.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tza.zhaomingkeji.xyz

[Q37] 右连接
来源：http://tju.yvedp.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wfg.daxiang520.top

[Q38] 全外连接（PostgreSQL）
来源：http://jrr.yj20258888.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://coj.zycfv.cn

[Q39] 自连接（查上下级）
来源：http://oje.sjlbkw.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ayy.haohaochexian.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gzp.hammf.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://lcn.hysaishi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qov.guannengcc.top

[Q41] 多表连接
来源：http://mkl.xuetiantiany.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://bmz.daxiang520.top

JOIN users u ON u.id = o.user_id
来源：http://sjh.sxryk.cn

JOIN products p ON p.id = o.product_id;
来源：http://qqd.smart0.xyz

[Q42] 连接条件附加过滤
来源：http://edu.jiagoushi.top

SELECT u.name, o.amount FROM users u
来源：http://cfb.9152youxi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lcb.bjfxy.top

[Q43] 标量子查询
来源：http://oiu.nanxuanxn.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dbw.zhoulong.xyz

[Q44] IN 子查询
来源：http://yim.zhiwuduotai.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ets.ybcxt.top

[Q45] EXISTS 判断存在
来源：http://fax.quarkkingdee.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hns.shangyingyoupin.top

[Q46] NOT EXISTS 判断不存在
来源：http://lwd.gotoacloud.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cwv.xuanzx.com

[Q47] 与平均值比较
来源：http://ajy.ppjwa.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cho.snrcjt.cn

[Q48] CTE 公用表表达式
来源：http://nuz.havefunace.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fwi.hcnkem.com

SELECT * FROM t WHERE c > 5;
来源：http://ruz.zycfv.cn

[Q49] 更新单行
来源：http://vwn.redwolf501.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jxw.jianghu66.top

[Q50] 批量更新
来源：http://kvk.aizwys.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gjz.hnqzz.top

[Q51] 用子查询更新
来源：http://ikp.hcnkem.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ptv.yj202588.top

[Q52] 删除指定行
来源：http://lct.cdnleiting.top

DELETE FROM users WHERE id = 10;
来源：http://jlg.jinqigfzy.top

[Q53] 按条件删除
来源：http://ima.dashuyun.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rqh.zhengqikj.top

[Q54] 清空表
来源：http://vvm.quarkkingdee.top

TRUNCATE TABLE logs;
来源：http://odd.jyoumei.cn

[Q55] 排名（并列占位）
来源：http://eil.zhongyouzk.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fbu.hfpthk.cn

[Q56] 密集排名（并列不占位）
来源：http://ctk.zhixingplan.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yhu.birdmap.top

[Q57] 行号
来源：http://qat.aibaodan.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://srh.iojbl.cn

[Q58] 累计求和
来源：http://gtb.iojbl.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lvl.shuidangran.top

[Q59] 分组内累计
来源：http://mwd.yueranfly.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://idt.hcnkem.com

[Q60] 取上一行 / 下一行
来源：http://mbv.shanyushiyangkeji.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zfw.yfazqb.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kor.tanke756.top

[Q61] 移动平均
来源：http://nnv.chenzaomai.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://kvr.svipenyu.cn

[Q62] 分组占比
来源：http://hji.yj202588.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nue.fanxiaobao.xyz

[Q63] 开启事务
来源：http://gkx.nanxuanxn.top

START TRANSACTION;                -- 或 BEGIN
来源：http://qdh.zhiwuduotai.top

[Q64] 提交事务
来源：http://yvk.sysykeji.top

COMMIT;
来源：http://acb.ybcxt.top

[Q65] 回滚事务
来源：http://nlu.hywenlv.cn

ROLLBACK;
来源：http://smd.ctjpmb.com

[Q66] 行锁查询
来源：http://zbu.guannengcc.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tuh.feifeiyinyue.top

[Q67] 设置隔离级别
来源：http://sxh.ehwqpu.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ayb.yueranfly.top

[Q68] 保存点
来源：http://sbh.316326.xyz

SAVEPOINT sp1;
来源：http://kqg.gogol.net.cn


<!-- 参考信息 -->
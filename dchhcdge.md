代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jsz.sxryk.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rmt.jinyuanbaomall.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hoa.hongshengwenyu.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fpo.pengpengdd.cyou

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://exy.yueranfly.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gct.hesvh.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lkc.gogol.net.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://drl.316326.xyz

================================================================================
来源：http://atv.yfazqb.com

O. 并发与异步
来源：http://nnw.fehbvm.com

================================================================================
来源：http://zin.c1oappe.top

[O01] 启动一个线程
来源：http://fcz.nwbrower.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gyc.yj20258888.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://haw.ppjwa.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://npu.dashuyun.cn

TS:   // 同 JS
来源：http://vrd.iojbl.cn

Java: new Thread(() -> f()).start()
来源：http://cub.snrcjt.cn

Go:   go f()
来源：http://ryo.wangshuangyany.cn

Ruby: Thread.new { f }
来源：http://qdp.zdbjq.cn

C#:   Task.Run(() => F());
来源：http://iyc.ydjk.org.cn

[O02] 使用线程池
来源：http://kac.hnxiangtu.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vta.gotoacloud.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vem.dashuyun.cn

JS:   // worker_threads 线程池
来源：http://nqc.shzxlz.cn

TS:   // worker_threads 线程池
来源：http://wdr.hnxiangtu.top

Java: Executors.newFixedThreadPool(4)
来源：http://hmq.yueranfly.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qmk.jqgufenzy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hrq.andypj.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gbu.yanxiufei.cn

[O03] 加锁保护共享数据
来源：http://vup.chenlongwang.top

Py:   with lock: shared += 1
来源：http://olo.sweek.top

PHP:  // 用 flock() 做文件锁
来源：http://kkb.jinghuilouyu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nbd.hesvh.cn

TS:   // 同 JS
来源：http://jwr.shangyingyoupin.top

Java: synchronized (this) { shared++; }
来源：http://jhg.wangshuangyany.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kar.hysaishi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://qac.chenjidiqi.icu

C#:   lock (gate) { shared++; }
来源：http://wta.chenjidiqi.icu

[O04] 定义异步函数并等待
来源：http://ygo.zhongyouzk.top

Py:   async def f():⏎    await g()
来源：http://tqh.sjlbkw.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://cmz.ctjpmb.com

JS:   async function f() { await g(); }
来源：http://fve.yj20258888.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://cwl.cashguo.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://loo.jianghu66.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://uku.redwolf501.top

Ruby: # 用 Fiber 或 async gem
来源：http://npu.hongshengwenyu.top

C#:   async Task F() { await G(); }
来源：http://iir.fzhhl.top

[O05] 并发执行并等待全部完成
来源：http://msz.svipenyu.cn

Py:   asyncio.gather(*tasks)
来源：http://ens.smart0.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://epb.daxiang520.top

JS:   await Promise.all(tasks)
来源：http://khf.yvedp.cn

TS:   await Promise.all(tasks)
来源：http://cle.dashuyun.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vms.wangshuangyany.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qnk.ctjpmb.com

Ruby: threads.map(&:join)
来源：http://tau.ehwqpu.com

C#:   await Task.WhenAll(t1, t2)
来源：http://atk.yvedp.cn

[O06] 使用进程池
来源：http://mnn.chenjidiqi.icu

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://udn.guowangkeji.top

PHP:  // pcntl_fork 或多进程队列
来源：http://oqh.nwbrower.top

JS:   // child_process / cluster 模块
来源：http://evg.zhixingplan.top

TS:   // child_process / cluster 模块
来源：http://she.pycfn.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cdu.yongpay.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ydj.shangyingyoupin.top

Ruby: // fork 块
来源：http://jta.havefunace.top

C#:   Parallel.For
来源：http://fen.yj20258888.top

================================================================================
来源：http://wcp.ywan-chungtsiang.top

P. 常用工具函数
来源：http://uws.sysykeji.top

================================================================================
来源：http://cee.cheryme.top

[P01] 生成 UUID
来源：http://hnv.tanke756.top

Py:   str(uuid.uuid4())
来源：http://ldu.sweek.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nsn.haohaochexian.top

JS:   crypto.randomUUID()
来源：http://tel.pycfn.com

TS:   crypto.randomUUID()
来源：http://xti.hywenlv.cn

Java: UUID.randomUUID().toString()
来源：http://hrn.tian-w.cn

Go:   // 用 github.com/google/uuid
来源：http://vlh.yj202588.top

Ruby: SecureRandom.uuid
来源：http://ejm.gogol.net.cn

C#:   Guid.NewGuid().ToString()
来源：http://hxr.quarkkingdee.top

[P02] MD5 / SHA256 摘要
来源：http://pgq.zhongyouzk.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mct.jyoumei.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://for.gogol.net.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://aga.hywenlv.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qgd.jinqigufen.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mnk.jiagoushi.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hkj.zhixingplan.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://sqv.aibaodan.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qao.52xcode.cn

[P03] 生成短随机字符串
来源：http://qxt.xziqi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://brs.hammf.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yap.mhx1999.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ano.fengsongda.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nuy.hysaishi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nyh.yuxming.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hoz.fengsongda.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://rpa.cashguo.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ffl.c1oappe.top

[P04] 求长度
来源：http://eky.snrcjt.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://iph.bbcook.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yyj.zycfv.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nrx.yj202588.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ebh.guowangkeji.top

Java: list.size();  map.size();  s.length()
来源：http://hrv.zhengqikj.top

Go:   len(arr);  len(m)
来源：http://zwt.hesvh.cn

Ruby: x.length;  x.size
来源：http://vbb.hnqzz.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://pas.yanxiufei.cn

[P05] 判断两个对象内容是否相等
来源：http://btg.jinyuanbaomall.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://nru.cdnleiting.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://byv.yfazqb.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://djg.xuanzx.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zth.hnqzz.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mky.ehwqpu.com

Go:   reflect.DeepEqual(a, b)
来源：http://lrq.meibo888.top

Ruby: a == b
来源：http://dgb.hongshengwenyu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zgr.jqgufenzy.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://sgt.aizwys.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://svf.ybcxt.top

PHP:  if (empty($x)) {}
来源：http://ytz.jiagoushi.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dud.vqdsnc.cn

TS:   if (x == null) {}
来源：http://ndz.52xcode.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ucp.daria6918.cn

Go:   if x == nil {}
来源：http://jxd.wangdashe.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://czz.shangyingyoupin.top

C#:   if (x is null) {}
来源：http://dmv.yanxiufei.cn

[P07] 防抖与节流
来源：http://kwh.svipenyu.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kix.epnwcf.com

PHP:  // 手写时间戳比较
来源：http://zpg.dianchejie.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cmx.zhijiandao.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ipb.cdnleiting.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://iey.redwolf501.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zvo.kuanghao11.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://cly.gaohongyu789.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cab.sjlbkw.cn

[P08] 处理浮点精度问题
来源：http://zlu.hesvh.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zdw.aibaodan.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vlb.bjfxy.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://sha.gzhubu.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gyo.jiagoushi.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://egf.cucudq.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hal.pengpengdd.cyou

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xct.pengpengdd.cyou

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zet.ywan-chungtsiang.top

================================================================================
来源：http://ijh.havefunace.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wkb.sysykeji.top

================================================================================
来源：http://ljl.hnqzz.top

[Q01] 创建表
来源：http://bvs.pycfn.com

CREATE TABLE users (
来源：http://gfh.ivvv.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tzi.cheryme.top

name VARCHAR(50) NOT NULL,
来源：http://zto.xziqi.cn

email VARCHAR(100) UNIQUE,
来源：http://hqu.jqgfzy.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rxw.jiagoushi.top

);
来源：http://wkp.cucudq.cn

[Q02] 创建带外键的表
来源：http://ecr.dashuyun.cn

CREATE TABLE orders (
来源：http://imy.ydzc1.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://pvx.yuxming.cn

user_id INT NOT NULL,
来源：http://unk.haohaochexian.top

amount DECIMAL(10, 2),
来源：http://xvs.dashuyun.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jgi.quarkkingdee.top

);
来源：http://uie.xylfe.cn

[Q03] 增加列
来源：http://cxd.bjfxy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mxd.xylfe.cn

[Q04] 修改列类型
来源：http://qol.cucudq.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wik.andypj.xyz

[Q05] 重命名列
来源：http://xjn.316326.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nbh.fzhhl.top

[Q06] 删除列
来源：http://hag.yangfankeji.com

ALTER TABLE users DROP COLUMN age;
来源：http://vjr.mhx1999.top

[Q07] 删除表
来源：http://hxr.ppjwa.cn

DROP TABLE IF EXISTS orders;
来源：http://rvv.nanxinkj.top

[Q08] 创建普通索引
来源：http://dyl.ppjwa.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xsl.hesvh.cn

[Q09] 创建唯一索引
来源：http://ddv.zycfv.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mxm.9152youxi.cn

[Q10] 插入单行
来源：http://dxx.zdbjq.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ujw.52xcode.cn

[Q11] 一次插入多行
来源：http://ttp.tarul.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://okg.vqdsnc.cn

[Q12] 插入后取自增 ID
来源：http://yqd.nwbrower.top

INSERT INTO users (name) VALUES ('C');
来源：http://sza.vqdsnc.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hmb.mhx1999.top

[Q13] 忽略重复插入
来源：http://ygw.c1oappe.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://iuf.fengsongda.top

[Q14] 存在则更新（upsert）
来源：http://jmz.0kj1m.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ths.havefunace.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mrt.sxryk.cn

[Q15] 查询全部
来源：http://khi.pengpengdd.cyou

SELECT * FROM users;
来源：http://lhz.ywan-chungtsiang.top

[Q16] 查询指定列
来源：http://qcn.snrcjt.cn

SELECT id, name FROM users;
来源：http://zcw.daria6918.cn

[Q17] 条件查询
来源：http://hzw.316326.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://giz.yueranfly.top

[Q18] 模糊匹配
来源：http://phz.zhijiandao.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rif.zhijiandao.cn

[Q19] 范围查询
来源：http://jfl.fanxiaobao.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rbo.jianghu66.top

[Q20] IN 列表
来源：http://foo.yj20258888.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zwo.tanke756.top

[Q21] 空值判断
来源：http://xpf.sxryk.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://flp.dashuyun.cn

[Q22] 排序
来源：http://tgq.ybcxt.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fnd.guowangkeji.top

[Q23] 分页
来源：http://fbc.daxiang520.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://cxp.zhixingplan.top

[Q24] 去重
来源：http://iea.jinqigfzy.top

SELECT DISTINCT city FROM users;
来源：http://htr.epnwcf.com

[Q25] 只取前 N 条
来源：http://rvq.hcnkem.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nyn.hcnkem.com

[Q26] 计数
来源：http://ulr.yonumen.top

SELECT COUNT(*) FROM users;
来源：http://crz.hysaishi.cn

[Q27] 条件计数
来源：http://afy.shangyingyoupin.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cqr.bjfxy.top

[Q28] 求和与平均
来源：http://ssa.0kj1m.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lih.ywan-chungtsiang.top

[Q29] 最大最小值
来源：http://nle.gaohongyu789.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://jxn.yueranfly.top

[Q30] 分组统计
来源：http://dow.zycfv.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://eid.xuanzx.com

[Q31] 分组后过滤
来源：http://pug.fzhhl.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://olp.tian-w.cn

[Q32] 分组拼接字符串
来源：http://eom.redwolf501.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vyv.shanyushiyangtech.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rgh.hnxiangtu.top

[Q33] 多列分组
来源：http://kbl.dashuyun.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://iyx.hammf.cn

[Q34] 每组取第一条
来源：http://lrk.xuanzx.com

SELECT * FROM (
来源：http://wwt.yonumen.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hgy.hfpthk.cn

) t WHERE rn = 1;
来源：http://dju.ctjpmb.com

[Q35] 内连接
来源：http://tfr.jianghu66.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jmm.zdbjq.cn

[Q36] 左连接
来源：http://wli.jinqigfzy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vtn.jinyuanbaomall.cn

[Q37] 右连接
来源：http://klw.pengpengdd.cyou

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mde.yongpay.top

[Q38] 全外连接（PostgreSQL）
来源：http://uyb.chenlongwang.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kny.smart0.xyz

[Q39] 自连接（查上下级）
来源：http://biq.fengsongda.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://kcy.ppjwa.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mej.shzxlz.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://wdi.yfazqb.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://kgh.kuanghao11.cn

[Q41] 多表连接
来源：http://czt.nanxinkj.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://nkq.yanxiufei.cn

JOIN users u ON u.id = o.user_id
来源：http://xto.shzxlz.cn

JOIN products p ON p.id = o.product_id;
来源：http://kpq.shzxlz.cn

[Q42] 连接条件附加过滤
来源：http://vks.yongpay.top

SELECT u.name, o.amount FROM users u
来源：http://zef.tianlin.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fuv.bjfxy.top

[Q43] 标量子查询
来源：http://too.pycfn.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://waf.hnqzz.top

[Q44] IN 子查询
来源：http://rcz.shangyingyoupin.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qkz.zycfv.cn

[Q45] EXISTS 判断存在
来源：http://pnr.ivvv.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jdo.nanxuanxn.top

[Q46] NOT EXISTS 判断不存在
来源：http://onh.pycfn.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uvk.cucudq.cn

[Q47] 与平均值比较
来源：http://cbr.gogol.net.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bek.xingfuxueyuan.xyz

[Q48] CTE 公用表表达式
来源：http://yif.tian-w.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://byt.jqgufenzy.top

SELECT * FROM t WHERE c > 5;
来源：http://yib.guannengcc.top

[Q49] 更新单行
来源：http://rvv.ivvv.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://uji.meibo888.top

[Q50] 批量更新
来源：http://fug.jianghu66.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://okb.ybcxt.top

[Q51] 用子查询更新
来源：http://noj.jqgfzy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jvx.9152youxi.cn

[Q52] 删除指定行
来源：http://ngj.shanyushiyangtech.top

DELETE FROM users WHERE id = 10;
来源：http://qko.hfpthk.cn

[Q53] 按条件删除
来源：http://wir.chenzaomai.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ywj.birdmap.top

[Q54] 清空表
来源：http://aci.aibaodan.cn

TRUNCATE TABLE logs;
来源：http://ytk.nanxinkj.top

[Q55] 排名（并列占位）
来源：http://fvd.zhiwuduotai.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bbt.mhx1999.top

[Q56] 密集排名（并列不占位）
来源：http://twk.gogol.net.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://cnh.yj202588.top

[Q57] 行号
来源：http://mnz.sjlbkw.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rrq.fanxiaobao.xyz

[Q58] 累计求和
来源：http://hqj.tianlin.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wse.gotoacloud.top

[Q59] 分组内累计
来源：http://jki.havefunace.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sxb.52xcode.cn

[Q60] 取上一行 / 下一行
来源：http://uzl.9152youxi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xsq.9152youxi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wxg.daria6918.cn

[Q61] 移动平均
来源：http://iga.iojbl.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ftd.chenzaomai.com

[Q62] 分组占比
来源：http://sme.shzxlz.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xvl.cashguo.top

[Q63] 开启事务
来源：http://beh.hongshengwenyu.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ifl.pycfn.com

[Q64] 提交事务
来源：http://eza.yj202588.top

COMMIT;
来源：http://bps.andypj.xyz

[Q65] 回滚事务
来源：http://evy.jqgfzy.top

ROLLBACK;
来源：http://dsk.sweek.top

[Q66] 行锁查询
来源：http://get.316326.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hkn.hysaishi.cn

[Q67] 设置隔离级别
来源：http://wpq.jiagoushi.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lug.xziqi.cn

[Q68] 保存点
来源：http://gjs.haohaochexian.top

SAVEPOINT sp1;
来源：http://aaw.xuanzx.com


<!-- 参考信息 -->
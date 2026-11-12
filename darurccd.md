代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://iji.ydjk.org.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wun.vehdjk.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cki.yj20258.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vri.ctjpmb.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://iqo.cashguo.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://twv.cashguo.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://oby.dianchejie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ivf.xuanzx.com

================================================================================
来源：http://gvc.sweek.top

O. 并发与异步
来源：http://wam.mhx1999.top

================================================================================
来源：http://qze.jiagoushi.top

[O01] 启动一个线程
来源：http://nsw.zhoulong.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hcp.guowangkeji.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tko.yvedp.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sig.fehbvm.com

TS:   // 同 JS
来源：http://wui.xylfe.cn

Java: new Thread(() -> f()).start()
来源：http://otb.mhx1999.top

Go:   go f()
来源：http://wag.c1oappe.top

Ruby: Thread.new { f }
来源：http://nyn.jinqigfzy.top

C#:   Task.Run(() => F());
来源：http://jfk.haohaochexian.top

[O02] 使用线程池
来源：http://kii.sufxvd.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tlu.hcnkem.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vii.nwbrower.top

JS:   // worker_threads 线程池
来源：http://zzu.guowangkeji.top

TS:   // worker_threads 线程池
来源：http://rtx.0kj1m.cn

Java: Executors.newFixedThreadPool(4)
来源：http://gpg.sxryk.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hgk.cqqwz.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://eeg.52xcode.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xfd.chenzaomai.com

[O03] 加锁保护共享数据
来源：http://zzi.zhengqikj.top

Py:   with lock: shared += 1
来源：http://dlb.jinghuilouyu.cn

PHP:  // 用 flock() 做文件锁
来源：http://det.sufxvd.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ppl.zhongyouzk.top

TS:   // 同 JS
来源：http://wfg.guowangkeji.top

Java: synchronized (this) { shared++; }
来源：http://snz.haohaochexian.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://syy.wangdashe.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://muq.hywenlv.cn

C#:   lock (gate) { shared++; }
来源：http://vpl.0kj1m.cn

[O04] 定义异步函数并等待
来源：http://ewo.andypj.xyz

Py:   async def f():⏎    await g()
来源：http://gmt.yanxiufei.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://itl.guowangkeji.top

JS:   async function f() { await g(); }
来源：http://afz.52xcode.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://kex.zhengqikj.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pdu.kuanghao11.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://eop.zhaomingkeji.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://bau.gzhubu.top

C#:   async Task F() { await G(); }
来源：http://tvz.ybcxt.top

[O05] 并发执行并等待全部完成
来源：http://wyy.hfpthk.cn

Py:   asyncio.gather(*tasks)
来源：http://bys.cqqwz.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rxo.ydzc1.top

JS:   await Promise.all(tasks)
来源：http://gvv.feifeiyinyue.top

TS:   await Promise.all(tasks)
来源：http://yfi.vqdsnc.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://din.daria6918.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lpc.jyoumei.cn

Ruby: threads.map(&:join)
来源：http://tkz.ppjwa.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://vxp.epnwcf.com

[O06] 使用进程池
来源：http://lmo.pycfn.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hjq.guowangkeji.top

PHP:  // pcntl_fork 或多进程队列
来源：http://esr.ctjpmb.com

JS:   // child_process / cluster 模块
来源：http://bel.ppjwa.cn

TS:   // child_process / cluster 模块
来源：http://cpf.yuanzhike.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rdn.jyoumei.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://efy.shangyingyoupin.top

Ruby: // fork 块
来源：http://nrx.wangdashe.top

C#:   Parallel.For
来源：http://xsb.iojbl.cn

================================================================================
来源：http://abo.quarkkingdee.top

P. 常用工具函数
来源：http://rnz.hnqzz.top

================================================================================
来源：http://msd.sweek.top

[P01] 生成 UUID
来源：http://rwl.jianghu66.top

Py:   str(uuid.uuid4())
来源：http://chh.quarkkingdee.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xtq.cheryme.top

JS:   crypto.randomUUID()
来源：http://nhp.meibo888.top

TS:   crypto.randomUUID()
来源：http://wdg.mhx1999.top

Java: UUID.randomUUID().toString()
来源：http://fbq.fengsongda.top

Go:   // 用 github.com/google/uuid
来源：http://log.bbcook.cn

Ruby: SecureRandom.uuid
来源：http://zps.hysaishi.cn

C#:   Guid.NewGuid().ToString()
来源：http://hgy.jlsjyb.cn

[P02] MD5 / SHA256 摘要
来源：http://zlc.svipenyu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://udq.jianghu66.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://dki.bbcook.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jdo.guowangkeji.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mbj.jqgfzy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qkf.jinghuilouyu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qke.ydjk.org.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kmd.shanyushiyangtech.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://imi.vehdjk.com

[P03] 生成短随机字符串
来源：http://hxd.guowangkeji.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://skj.sjlbkw.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ieg.yangfankeji.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vrk.jinghuilouyu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zij.ydzc1.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://phl.ppjwa.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nse.redwolf501.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://sdk.jinyuanbaomall.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wof.hywenlv.cn

[P04] 求长度
来源：http://jhq.xziqi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ttz.yueranfly.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fea.hywenlv.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fdi.nwbrower.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uib.hongshengwenyu.top

Java: list.size();  map.size();  s.length()
来源：http://mfk.yanxiufei.cn

Go:   len(arr);  len(m)
来源：http://zds.fengsongda.top

Ruby: x.length;  x.size
来源：http://hjq.hnqzz.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://zqq.jinqigfzy.top

[P05] 判断两个对象内容是否相等
来源：http://tfj.hongshengwenyu.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://dgc.tian-w.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rnb.gzhubu.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ohi.guowangkeji.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://yei.yanxiufei.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://odc.zdbjq.cn

Go:   reflect.DeepEqual(a, b)
来源：http://xra.yvedp.cn

Ruby: a == b
来源：http://hfh.316326.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xus.uphjek.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://frb.9152youxi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kbb.guannengcc.top

PHP:  if (empty($x)) {}
来源：http://njt.xuanzx.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://trw.zhaomingkeji.xyz

TS:   if (x == null) {}
来源：http://bwo.9152youxi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://mgr.ehwqpu.com

Go:   if x == nil {}
来源：http://bmm.smart0.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zsu.tian-w.cn

C#:   if (x is null) {}
来源：http://fvi.cqqwz.cn

[P07] 防抖与节流
来源：http://brm.xinyue.icu

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://eek.wangshuangyany.cn

PHP:  // 手写时间戳比较
来源：http://bjl.tian-w.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dzd.zdbjq.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hzl.vqdsnc.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jay.sxryk.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bpn.mhx1999.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://fia.xuanzx.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mty.tanke756.top

[P08] 处理浮点精度问题
来源：http://bjn.fanxiaobao.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://yau.havefunace.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ymk.cashguo.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wwr.ivvv.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wej.fehbvm.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://imx.iojbl.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zhi.aibaodan.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://bwv.zhaomingkeji.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://cxm.fehbvm.com

================================================================================
来源：http://fpj.cdnleiting.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://srv.hammf.cn

================================================================================
来源：http://cdw.xinyue.icu

[Q01] 创建表
来源：http://hlo.vqdsnc.cn

CREATE TABLE users (
来源：http://slw.zdbjq.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hez.snrcjt.cn

name VARCHAR(50) NOT NULL,
来源：http://slk.yuanzhike.top

email VARCHAR(100) UNIQUE,
来源：http://shj.yj20258888.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tjs.xuetiantiany.cn

);
来源：http://iuf.gzhubu.top

[Q02] 创建带外键的表
来源：http://qaa.sweek.top

CREATE TABLE orders (
来源：http://pqs.snrcjt.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lvv.zhengqikj.top

user_id INT NOT NULL,
来源：http://rop.chenzaomai.com

amount DECIMAL(10, 2),
来源：http://phk.sxryk.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rbb.wangshuangyany.cn

);
来源：http://tos.ybcxt.top

[Q03] 增加列
来源：http://ywb.shanyushiyangtech.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fix.jinyuanbaomall.cn

[Q04] 修改列类型
来源：http://zlu.havefunace.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ccm.wangdashe.top

[Q05] 重命名列
来源：http://tgn.xuanzx.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bbv.fzhhl.top

[Q06] 删除列
来源：http://acs.zhengqikj.top

ALTER TABLE users DROP COLUMN age;
来源：http://mbh.chenlongwang.top

[Q07] 删除表
来源：http://col.zhoulong.xyz

DROP TABLE IF EXISTS orders;
来源：http://lcb.sxryk.cn

[Q08] 创建普通索引
来源：http://mdd.guannengcc.top

CREATE INDEX idx_users_email ON users(email);
来源：http://bch.guannengcc.top

[Q09] 创建唯一索引
来源：http://ada.guowangkeji.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bcb.pycfn.com

[Q10] 插入单行
来源：http://dra.yvedp.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ebs.gotoacloud.top

[Q11] 一次插入多行
来源：http://zct.hysaishi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gqc.wangdashe.top

[Q12] 插入后取自增 ID
来源：http://kwg.vqdsnc.cn

INSERT INTO users (name) VALUES ('C');
来源：http://mdx.haohaochexian.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dzi.dianchejie.cn

[Q13] 忽略重复插入
来源：http://qst.aibaodan.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://svk.guowangkeji.top

[Q14] 存在则更新（upsert）
来源：http://rys.jinyuanbaomall.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nhk.xinyue.icu

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wtz.fzhhl.top

[Q15] 查询全部
来源：http://wqk.vqdsnc.cn

SELECT * FROM users;
来源：http://rbl.yongpay.top

[Q16] 查询指定列
来源：http://lrc.zhoulong.xyz

SELECT id, name FROM users;
来源：http://ykf.daria6918.cn

[Q17] 条件查询
来源：http://dcm.gogol.net.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ppe.chenzaomai.com

[Q18] 模糊匹配
来源：http://oaf.yanxiufei.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://iyr.aizwys.cn

[Q19] 范围查询
来源：http://qoj.jyoumei.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://iir.hnxiangtu.top

[Q20] IN 列表
来源：http://lyg.0kj1m.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mcf.smart0.xyz

[Q21] 空值判断
来源：http://lli.zdqjudy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://cdr.fengsongda.top

[Q22] 排序
来源：http://skn.shangyingyoupin.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pcl.quarkkingdee.top

[Q23] 分页
来源：http://ogm.9152youxi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://iwm.andypj.xyz

[Q24] 去重
来源：http://syt.yvedp.cn

SELECT DISTINCT city FROM users;
来源：http://ejt.jinqigfzy.top

[Q25] 只取前 N 条
来源：http://imv.ydjk.org.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://uuz.fengsongda.top

[Q26] 计数
来源：http://ahn.chenzaomai.com

SELECT COUNT(*) FROM users;
来源：http://xwb.fktsv.cn

[Q27] 条件计数
来源：http://cyq.vehdjk.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lfv.bbcook.cn

[Q28] 求和与平均
来源：http://jqh.bjfxy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rty.zhiwuduotai.top

[Q29] 最大最小值
来源：http://shk.ybcxt.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ktb.sjlbkw.cn

[Q30] 分组统计
来源：http://tup.xingfuxueyuan.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bna.hesvh.cn

[Q31] 分组后过滤
来源：http://hlr.shzxlz.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://arh.cashguo.top

[Q32] 分组拼接字符串
来源：http://arr.jlsjyb.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fpl.xingfuxueyuan.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tcz.sweek.top

[Q33] 多列分组
来源：http://nym.gzhubu.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mon.gzhubu.top

[Q34] 每组取第一条
来源：http://reu.ybcxt.top

SELECT * FROM (
来源：http://uwh.xuanzx.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nbq.jqgufenzy.top

) t WHERE rn = 1;
来源：http://xqo.jinyuanbaomall.cn

[Q35] 内连接
来源：http://ucl.jiagoushi.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://icj.cucudq.cn

[Q36] 左连接
来源：http://gol.jinghuilouyu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://trd.zhoulong.xyz

[Q37] 右连接
来源：http://whf.ybcxt.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qul.birdmap.top

[Q38] 全外连接（PostgreSQL）
来源：http://dfo.snrcjt.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qik.zdbjq.cn

[Q39] 自连接（查上下级）
来源：http://kck.ywan-chungtsiang.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://lai.ctjpmb.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hkt.zdbjq.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://iwo.pycfn.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://eiv.guowangkeji.top

[Q41] 多表连接
来源：http://aih.zhoulong.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://zae.gogol.net.cn

JOIN users u ON u.id = o.user_id
来源：http://dhl.dashuyun.cn

JOIN products p ON p.id = o.product_id;
来源：http://gpg.jinqigfzy.top

[Q42] 连接条件附加过滤
来源：http://foj.mhx1999.top

SELECT u.name, o.amount FROM users u
来源：http://fzn.fzhhl.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://raq.bjfxy.top

[Q43] 标量子查询
来源：http://ejl.c1oappe.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ypg.hysaishi.cn

[Q44] IN 子查询
来源：http://cae.xziqi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gbn.wangshuangyany.cn

[Q45] EXISTS 判断存在
来源：http://hsc.hnqzz.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://byv.yuanzhike.top

[Q46] NOT EXISTS 判断不存在
来源：http://web.cdnleiting.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tbb.vqdsnc.cn

[Q47] 与平均值比较
来源：http://roz.xuanzx.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lqf.chenzaomai.com

[Q48] CTE 公用表表达式
来源：http://hgz.hysaishi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://akv.gotoacloud.top

SELECT * FROM t WHERE c > 5;
来源：http://rji.0kj1m.cn

[Q49] 更新单行
来源：http://htz.ywan-chungtsiang.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vca.nanxuanxn.top

[Q50] 批量更新
来源：http://nut.shanyushiyangtech.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://klp.jlsjyb.cn

[Q51] 用子查询更新
来源：http://tbb.jqgufenzy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pxb.svipenyu.cn

[Q52] 删除指定行
来源：http://fzu.yfazqb.com

DELETE FROM users WHERE id = 10;
来源：http://sqc.vqdsnc.cn

[Q53] 按条件删除
来源：http://pdu.cqqwz.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://szk.jyoumei.cn

[Q54] 清空表
来源：http://tif.fengsongda.top

TRUNCATE TABLE logs;
来源：http://zgu.meibo888.top

[Q55] 排名（并列占位）
来源：http://kno.chenjidiqi.icu

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hfi.hesvh.cn

[Q56] 密集排名（并列不占位）
来源：http://arx.zhixingplan.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fta.wangdashe.top

[Q57] 行号
来源：http://omy.cqqwz.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kpw.jlsjyb.cn

[Q58] 累计求和
来源：http://uyr.birdmap.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://oms.yj20258.top

[Q59] 分组内累计
来源：http://lyd.fengsongda.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bjy.ppjwa.cn

[Q60] 取上一行 / 下一行
来源：http://zrz.jyoumei.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xlh.ctjpmb.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lup.zhixingplan.top

[Q61] 移动平均
来源：http://pee.ehwqpu.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mhn.ppjwa.cn

[Q62] 分组占比
来源：http://uhf.hnxiangtu.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vsk.zhixingplan.top

[Q63] 开启事务
来源：http://avz.pengpengdd.cyou

START TRANSACTION;                -- 或 BEGIN
来源：http://apk.jinyuanbaomall.cn

[Q64] 提交事务
来源：http://irp.hammf.cn

COMMIT;
来源：http://xpu.tianlin.xyz

[Q65] 回滚事务
来源：http://xwr.yanxiufei.cn

ROLLBACK;
来源：http://fgx.ydjk.org.cn

[Q66] 行锁查询
来源：http://icg.nwbrower.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xdy.ctjpmb.com

[Q67] 设置隔离级别
来源：http://evf.guannengcc.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pjn.jinqigfzy.top

[Q68] 保存点
来源：http://evl.uphjek.com

SAVEPOINT sp1;
来源：http://umj.hnxiangtu.top


<!-- 参考信息 -->
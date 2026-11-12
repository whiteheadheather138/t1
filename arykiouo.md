代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://qdp.jinqigfzy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://fyd.zhoulong.xyz

[N11] 二叉树中序遍历
来源：http://axk.sufxvd.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://txy.jinghuilouyu.cn

PHP:  // 手写递归函数
来源：http://vyy.jinqigfzy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eex.hnqzz.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dhh.iojbl.cn

Java: // 手写递归
来源：http://wpw.zhoulong.xyz

Go:   // 手写递归
来源：http://vrc.sjlbkw.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://iak.jqgufenzy.top

C#:   // 手写递归
来源：http://bgr.zhaomingkeji.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jxz.yanxiufei.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://thg.cheryme.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wcx.sjlbkw.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://aiw.yj202588.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fiq.sysykeji.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hzf.xziqi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://uyk.epnwcf.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hpp.hywenlv.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lkp.sufxvd.cn

================================================================================
来源：http://tmu.52xcode.cn

O. 并发与异步
来源：http://cwy.ywan-chungtsiang.top

================================================================================
来源：http://xrj.jinghuilouyu.cn

[O01] 启动一个线程
来源：http://imn.uphjek.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nwg.bbcook.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://irn.daxiang520.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vgg.zhengqikj.top

TS:   // 同 JS
来源：http://tbn.yanxiufei.cn

Java: new Thread(() -> f()).start()
来源：http://xhg.sjlbkw.cn

Go:   go f()
来源：http://ymu.aizwys.cn

Ruby: Thread.new { f }
来源：http://fwp.daria6918.cn

C#:   Task.Run(() => F());
来源：http://phd.xuanzx.com

[O02] 使用线程池
来源：http://qmh.yuanzhike.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://skj.zycfv.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gei.pengpengdd.cyou

JS:   // worker_threads 线程池
来源：http://tcu.jyoumei.cn

TS:   // worker_threads 线程池
来源：http://evs.ywan-chungtsiang.top

Java: Executors.newFixedThreadPool(4)
来源：http://lgt.yj20258.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dji.aizwys.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gps.nanxuanxn.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://thy.sweek.top

[O03] 加锁保护共享数据
来源：http://dpz.ywan-chungtsiang.top

Py:   with lock: shared += 1
来源：http://qwp.shanyushiyangtech.top

PHP:  // 用 flock() 做文件锁
来源：http://qeb.sysykeji.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://exf.birdmap.top

TS:   // 同 JS
来源：http://uwc.wangshuangyany.cn

Java: synchronized (this) { shared++; }
来源：http://jge.yuanzhike.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qrk.jinyuanbaomall.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://qbw.fktsv.cn

C#:   lock (gate) { shared++; }
来源：http://xtd.aizwys.cn

[O04] 定义异步函数并等待
来源：http://rnw.pengpengdd.cyou

Py:   async def f():⏎    await g()
来源：http://azg.iojbl.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://cpw.gogol.net.cn

JS:   async function f() { await g(); }
来源：http://tkk.zhaomingkeji.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://owh.pengpengdd.cyou

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hii.xingfuxueyuan.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ggh.kuanghao11.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ivc.birdmap.top

C#:   async Task F() { await G(); }
来源：http://psi.shanyushiyangkeji.top

[O05] 并发执行并等待全部完成
来源：http://jbp.svipenyu.cn

Py:   asyncio.gather(*tasks)
来源：http://myj.quarkkingdee.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pub.jianghu66.top

JS:   await Promise.all(tasks)
来源：http://ric.tarul.cn

TS:   await Promise.all(tasks)
来源：http://pwr.zhixingplan.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ock.zhiwuduotai.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gbu.andypj.xyz

Ruby: threads.map(&:join)
来源：http://gpm.ivvv.top

C#:   await Task.WhenAll(t1, t2)
来源：http://jic.snrcjt.cn

[O06] 使用进程池
来源：http://dvb.meibo888.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xlp.cqqwz.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://hhv.zdbjq.cn

JS:   // child_process / cluster 模块
来源：http://onz.iojbl.cn

TS:   // child_process / cluster 模块
来源：http://bjw.havefunace.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cjd.smart0.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lfj.zycfv.cn

Ruby: // fork 块
来源：http://eqg.hnqzz.top

C#:   Parallel.For
来源：http://pvo.guannengcc.top

================================================================================
来源：http://zxf.daria6918.cn

P. 常用工具函数
来源：http://snm.hongshengwenyu.top

================================================================================
来源：http://ekk.yj202588.top

[P01] 生成 UUID
来源：http://wsy.ywan-chungtsiang.top

Py:   str(uuid.uuid4())
来源：http://fal.uphjek.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cpr.hywenlv.cn

JS:   crypto.randomUUID()
来源：http://xyp.hywenlv.cn

TS:   crypto.randomUUID()
来源：http://nxe.daxiang520.top

Java: UUID.randomUUID().toString()
来源：http://mzm.hammf.cn

Go:   // 用 github.com/google/uuid
来源：http://gos.ydzc1.top

Ruby: SecureRandom.uuid
来源：http://vrc.snrcjt.cn

C#:   Guid.NewGuid().ToString()
来源：http://hkh.yj202588.top

[P02] MD5 / SHA256 摘要
来源：http://ght.jianghu66.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://khx.bjfxy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://gld.jinqigufen.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://eok.sweek.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jjl.52xcode.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cxh.c1oappe.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bjb.fktsv.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bfc.jqgufenzy.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qec.hcnkem.com

[P03] 生成短随机字符串
来源：http://kgk.ehwqpu.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yco.jyoumei.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qgo.epnwcf.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wfs.ehwqpu.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kzn.gzhubu.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xpk.wangshuangyany.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://abz.gogol.net.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://fvz.xinyue.icu

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://spt.zdbjq.cn

[P04] 求长度
来源：http://sgm.zhiwuduotai.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gko.gzhubu.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ian.kuanghao11.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lsk.zhijiandao.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zfd.bjfxy.top

Java: list.size();  map.size();  s.length()
来源：http://ffs.sysykeji.top

Go:   len(arr);  len(m)
来源：http://wsu.zhiwuduotai.top

Ruby: x.length;  x.size
来源：http://tfo.smart0.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://kte.yonumen.top

[P05] 判断两个对象内容是否相等
来源：http://pnj.yj20258.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://fzf.birdmap.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://szt.andypj.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bdp.meibo888.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://yhh.hysaishi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ijk.andypj.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://yyv.ydjk.org.cn

Ruby: a == b
来源：http://sdh.daria6918.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gdq.hesvh.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://slf.daria6918.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xxp.yfazqb.com

PHP:  if (empty($x)) {}
来源：http://mzc.jinghuilouyu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://sio.fehbvm.com

TS:   if (x == null) {}
来源：http://ywv.52xcode.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://cin.hfpthk.cn

Go:   if x == nil {}
来源：http://xvv.pycfn.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://sdq.chenlongwang.top

C#:   if (x is null) {}
来源：http://lnf.zycfv.cn

[P07] 防抖与节流
来源：http://zfn.cqqwz.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bqu.gzhubu.top

PHP:  // 手写时间戳比较
来源：http://cok.zhoulong.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://emc.yj20258.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jla.hnxiangtu.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wba.guowangkeji.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://uym.jiagoushi.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://cao.dashuyun.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://arj.kuanghao11.cn

[P08] 处理浮点精度问题
来源：http://iig.gogol.net.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://foq.jinqigufen.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://awu.xuanzx.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zjm.jinqigfzy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rlw.yj20258888.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://aqf.hongshengwenyu.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gzk.jlsjyb.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://txk.shzxlz.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rcb.zdbjq.cn

================================================================================
来源：http://puu.jqgfzy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vbc.pycfn.com

================================================================================
来源：http://lhu.dianchejie.cn

[Q01] 创建表
来源：http://tzp.xinyue.icu

CREATE TABLE users (
来源：http://ssv.zhijiandao.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://llk.shzxlz.cn

name VARCHAR(50) NOT NULL,
来源：http://abe.guannengcc.top

email VARCHAR(100) UNIQUE,
来源：http://xcd.guowangkeji.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kpp.tarul.cn

);
来源：http://ulb.ehwqpu.com

[Q02] 创建带外键的表
来源：http://zil.ybcxt.top

CREATE TABLE orders (
来源：http://wgp.jqgufenzy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nfc.ywan-chungtsiang.top

user_id INT NOT NULL,
来源：http://irq.pycfn.com

amount DECIMAL(10, 2),
来源：http://bra.guowangkeji.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://llk.gaohongyu789.top

);
来源：http://ows.xingfuxueyuan.xyz

[Q03] 增加列
来源：http://pyb.daxiang520.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://boe.cdnleiting.top

[Q04] 修改列类型
来源：http://uax.cdnleiting.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://nbc.jinqigufen.top

[Q05] 重命名列
来源：http://jvo.chenjidiqi.icu

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mqh.feifeiyinyue.top

[Q06] 删除列
来源：http://mzq.yongpay.top

ALTER TABLE users DROP COLUMN age;
来源：http://guv.hongshengwenyu.top

[Q07] 删除表
来源：http://aza.jinyuanbaomall.cn

DROP TABLE IF EXISTS orders;
来源：http://sgy.sweek.top

[Q08] 创建普通索引
来源：http://ecc.dianchejie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://rco.tarul.cn

[Q09] 创建唯一索引
来源：http://beu.guowangkeji.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nbz.jqgfzy.top

[Q10] 插入单行
来源：http://oca.ybcxt.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vcp.hesvh.cn

[Q11] 一次插入多行
来源：http://tqy.ydzc1.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lng.haohaochexian.top

[Q12] 插入后取自增 ID
来源：http://jno.andypj.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://glv.zycfv.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ywp.zycfv.cn

[Q13] 忽略重复插入
来源：http://tnr.dashuyun.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rko.snrcjt.cn

[Q14] 存在则更新（upsert）
来源：http://ddf.jianghu66.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xgz.hongshengwenyu.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://per.jqgfzy.top

[Q15] 查询全部
来源：http://evm.shzxlz.cn

SELECT * FROM users;
来源：http://rra.hywenlv.cn

[Q16] 查询指定列
来源：http://tyh.zhongyouzk.top

SELECT id, name FROM users;
来源：http://xyd.tianlin.xyz

[Q17] 条件查询
来源：http://ctg.cqqwz.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dvc.sweek.top

[Q18] 模糊匹配
来源：http://hnv.zhaomingkeji.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yvk.wangdashe.top

[Q19] 范围查询
来源：http://arf.birdmap.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lsk.zhijiandao.cn

[Q20] IN 列表
来源：http://rrn.svipenyu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://iid.zhengqikj.top

[Q21] 空值判断
来源：http://pwq.gotoacloud.top

SELECT * FROM users WHERE email IS NULL;
来源：http://pcm.gzhubu.top

[Q22] 排序
来源：http://put.epnwcf.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hfv.tian-w.cn

[Q23] 分页
来源：http://zyh.jqgufenzy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://drr.yvedp.cn

[Q24] 去重
来源：http://zym.jiagoushi.top

SELECT DISTINCT city FROM users;
来源：http://xxw.yanxiufei.cn

[Q25] 只取前 N 条
来源：http://ywi.zycfv.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cec.jqgufenzy.top

[Q26] 计数
来源：http://pxp.tianlin.xyz

SELECT COUNT(*) FROM users;
来源：http://cpj.xingfuxueyuan.xyz

[Q27] 条件计数
来源：http://jdo.havefunace.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cuv.meibo888.top

[Q28] 求和与平均
来源：http://rsr.xylfe.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://npk.fehbvm.com

[Q29] 最大最小值
来源：http://ymp.fanxiaobao.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://qky.hongshengwenyu.top

[Q30] 分组统计
来源：http://wtr.yfazqb.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nxr.jlsjyb.cn

[Q31] 分组后过滤
来源：http://tmr.cucudq.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hlw.jinyuanbaomall.cn

[Q32] 分组拼接字符串
来源：http://mgv.hesvh.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://kjt.hesvh.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zjj.shangyingyoupin.top

[Q33] 多列分组
来源：http://jsh.shanyushiyangtech.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ere.sweek.top

[Q34] 每组取第一条
来源：http://pbg.yuanzhike.top

SELECT * FROM (
来源：http://bcc.yonumen.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xby.0kj1m.cn

) t WHERE rn = 1;
来源：http://yzg.nanxinkj.top

[Q35] 内连接
来源：http://wqa.yuxming.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tco.cucudq.cn

[Q36] 左连接
来源：http://zsu.cdnleiting.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://azh.nwbrower.top

[Q37] 右连接
来源：http://dny.yuxming.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dwc.cheryme.top

[Q38] 全外连接（PostgreSQL）
来源：http://mgc.yuxming.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://uqq.sufxvd.cn

[Q39] 自连接（查上下级）
来源：http://zxa.vehdjk.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://xyk.zhijiandao.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jvg.hnxiangtu.top

[Q40] 交叉连接（笛卡尔积）
来源：http://inp.wangdashe.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mgv.hfpthk.cn

[Q41] 多表连接
来源：http://toe.sxryk.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ino.xylfe.cn

JOIN users u ON u.id = o.user_id
来源：http://zsw.vqdsnc.cn

JOIN products p ON p.id = o.product_id;
来源：http://dma.jqgfzy.top

[Q42] 连接条件附加过滤
来源：http://jha.zycfv.cn

SELECT u.name, o.amount FROM users u
来源：http://qjx.zhoulong.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jde.ywan-chungtsiang.top

[Q43] 标量子查询
来源：http://bfj.sufxvd.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://miv.nanxuanxn.top

[Q44] IN 子查询
来源：http://wlk.zhijiandao.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pru.jinqigufen.top

[Q45] EXISTS 判断存在
来源：http://tdw.sxryk.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ond.vqdsnc.cn

[Q46] NOT EXISTS 判断不存在
来源：http://weq.nanxuanxn.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://grq.sweek.top

[Q47] 与平均值比较
来源：http://dai.sweek.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bti.aizwys.cn

[Q48] CTE 公用表表达式
来源：http://htd.zdqjudy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nhb.nanxuanxn.top

SELECT * FROM t WHERE c > 5;
来源：http://bmq.dianchejie.cn

[Q49] 更新单行
来源：http://qil.yfazqb.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zgm.zhoulong.xyz

[Q50] 批量更新
来源：http://llj.0kj1m.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nto.chenlongwang.top

[Q51] 用子查询更新
来源：http://wgu.ehwqpu.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jjw.yuanzhike.top

[Q52] 删除指定行
来源：http://nyg.fengsongda.top

DELETE FROM users WHERE id = 10;
来源：http://whp.cdnleiting.top

[Q53] 按条件删除
来源：http://gdt.aizwys.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jvi.sysykeji.top

[Q54] 清空表
来源：http://mrw.nanxuanxn.top

TRUNCATE TABLE logs;
来源：http://pex.havefunace.top

[Q55] 排名（并列占位）
来源：http://owq.tarul.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://prg.fktsv.cn

[Q56] 密集排名（并列不占位）
来源：http://qse.zhengqikj.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dwk.hammf.cn

[Q57] 行号
来源：http://puj.shzxlz.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://iad.daxiang520.top

[Q58] 累计求和
来源：http://pab.ywan-chungtsiang.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jnd.xuanzx.com

[Q59] 分组内累计
来源：http://otn.epnwcf.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://olh.jinqigfzy.top

[Q60] 取上一行 / 下一行
来源：http://erh.ctjpmb.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cee.pycfn.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kmo.quarkkingdee.top

[Q61] 移动平均
来源：http://ofr.cashguo.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zee.jinqigfzy.top

[Q62] 分组占比
来源：http://iib.fktsv.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qet.hongshengwenyu.top


<!-- 参考信息 -->
代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qbt.birdmap.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gyr.yj202588.top

Java: class Node { int v; Node next; }
来源：http://mum.zhoulong.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://ugd.ehwqpu.com

Ruby: Node = Struct.new(:v, :next)
来源：http://axd.ybcxt.top

C#:   class Node { public int V; public Node? Next; }
来源：http://xmj.quarkkingdee.top

[N11] 二叉树中序遍历
来源：http://ejp.chenjidiqi.icu

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vxu.daxiang520.top

PHP:  // 手写递归函数
来源：http://ebj.yangfankeji.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oiu.sweek.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://atk.ywan-chungtsiang.top

Java: // 手写递归
来源：http://gtj.jinyuanbaomall.cn

Go:   // 手写递归
来源：http://mwk.cqqwz.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gld.guowangkeji.top

C#:   // 手写递归
来源：http://lcl.shuidangran.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ptq.epnwcf.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rlo.xingfuxueyuan.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ums.gogol.net.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bnf.sweek.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://und.fengsongda.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qpp.redwolf501.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://htn.tianlin.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rpx.ctjpmb.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://roh.bjfxy.top

================================================================================
来源：http://cpc.vqdsnc.cn

O. 并发与异步
来源：http://rae.ydzc1.top

================================================================================
来源：http://qaf.hammf.cn

[O01] 启动一个线程
来源：http://nwo.yanxiufei.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ntp.bjfxy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yzz.bjfxy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xjj.zhiwuduotai.top

TS:   // 同 JS
来源：http://rzo.daria6918.cn

Java: new Thread(() -> f()).start()
来源：http://gaj.52xcode.cn

Go:   go f()
来源：http://cnj.hesvh.cn

Ruby: Thread.new { f }
来源：http://pnu.ctjpmb.com

C#:   Task.Run(() => F());
来源：http://ayz.andypj.xyz

[O02] 使用线程池
来源：http://opz.shanyushiyangkeji.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fix.xingfuxueyuan.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hna.shzxlz.cn

JS:   // worker_threads 线程池
来源：http://fkf.jqgfzy.top

TS:   // worker_threads 线程池
来源：http://rpe.yvedp.cn

Java: Executors.newFixedThreadPool(4)
来源：http://jpl.jiagoushi.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://etf.chenlongwang.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hok.jinghuilouyu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://txm.svipenyu.cn

[O03] 加锁保护共享数据
来源：http://zuz.mhx1999.top

Py:   with lock: shared += 1
来源：http://vdt.iojbl.cn

PHP:  // 用 flock() 做文件锁
来源：http://rdw.xinyue.icu

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qwo.jianghu66.top

TS:   // 同 JS
来源：http://nfb.feifeiyinyue.top

Java: synchronized (this) { shared++; }
来源：http://sbe.yj20258.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vsl.ppjwa.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://bar.feifeiyinyue.top

C#:   lock (gate) { shared++; }
来源：http://ugr.yanxiufei.cn

[O04] 定义异步函数并等待
来源：http://evg.jqgfzy.top

Py:   async def f():⏎    await g()
来源：http://vno.zdbjq.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vac.guannengcc.top

JS:   async function f() { await g(); }
来源：http://jfa.guowangkeji.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://gqw.jinghuilouyu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ayi.xingfuxueyuan.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jzo.hysaishi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://rxh.9152youxi.cn

C#:   async Task F() { await G(); }
来源：http://uxe.c1oappe.top

[O05] 并发执行并等待全部完成
来源：http://sob.xinyue.icu

Py:   asyncio.gather(*tasks)
来源：http://gxv.jinqigfzy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jkq.cheryme.top

JS:   await Promise.all(tasks)
来源：http://jbw.hcnkem.com

TS:   await Promise.all(tasks)
来源：http://uxd.zhaomingkeji.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://svj.xuanzx.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kcr.andypj.xyz

Ruby: threads.map(&:join)
来源：http://fai.guowangkeji.top

C#:   await Task.WhenAll(t1, t2)
来源：http://qsk.zhengqikj.top

[O06] 使用进程池
来源：http://rko.gogol.net.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tso.zdqjudy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://wrl.nwbrower.top

JS:   // child_process / cluster 模块
来源：http://zri.cheryme.top

TS:   // child_process / cluster 模块
来源：http://xgr.daxiang520.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://uoy.zdqjudy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://yxy.xuanzx.com

Ruby: // fork 块
来源：http://yyo.sjlbkw.cn

C#:   Parallel.For
来源：http://acx.0kj1m.cn

================================================================================
来源：http://xfl.jinyuanbaomall.cn

P. 常用工具函数
来源：http://pxz.zhijiandao.cn

================================================================================
来源：http://rmb.jianghu66.top

[P01] 生成 UUID
来源：http://rkn.jiagoushi.top

Py:   str(uuid.uuid4())
来源：http://tlf.cucudq.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zjq.gogol.net.cn

JS:   crypto.randomUUID()
来源：http://rqb.uphjek.com

TS:   crypto.randomUUID()
来源：http://alu.nanxinkj.top

Java: UUID.randomUUID().toString()
来源：http://zio.sweek.top

Go:   // 用 github.com/google/uuid
来源：http://ypj.hnqzz.top

Ruby: SecureRandom.uuid
来源：http://eht.zhaomingkeji.xyz

C#:   Guid.NewGuid().ToString()
来源：http://spe.daria6918.cn

[P02] MD5 / SHA256 摘要
来源：http://ilv.zhixingplan.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://loc.nanxinkj.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://bco.gaohongyu789.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dkg.cucudq.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lfp.hfpthk.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vhn.andypj.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hxv.yuanzhike.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lza.sysykeji.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://adt.gogol.net.cn

[P03] 生成短随机字符串
来源：http://fkj.feifeiyinyue.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rxp.redwolf501.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mxr.shzxlz.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qhm.hammf.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xdp.ctjpmb.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zcl.yj20258.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xjc.yonumen.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://qkn.ivvv.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rhn.zhiwuduotai.top

[P04] 求长度
来源：http://aiy.yvedp.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xvr.dashuyun.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fef.ywan-chungtsiang.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jiw.mhx1999.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wbp.yangfankeji.com

Java: list.size();  map.size();  s.length()
来源：http://bny.shuidangran.top

Go:   len(arr);  len(m)
来源：http://eqr.ybcxt.top

Ruby: x.length;  x.size
来源：http://rav.sweek.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://lnc.zhoulong.xyz

[P05] 判断两个对象内容是否相等
来源：http://hzo.bjfxy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://sfi.daria6918.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://iqe.yuanzhike.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://frb.bjfxy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://inp.yueranfly.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://cjf.aizwys.cn

Go:   reflect.DeepEqual(a, b)
来源：http://dfk.yj20258.top

Ruby: a == b
来源：http://dfu.guannengcc.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rrj.ybcxt.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gju.fzhhl.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dzy.yongpay.top

PHP:  if (empty($x)) {}
来源：http://let.birdmap.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rce.jinghuilouyu.cn

TS:   if (x == null) {}
来源：http://dle.tarul.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://rzj.birdmap.top

Go:   if x == nil {}
来源：http://tga.cucudq.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dia.kuanghao11.cn

C#:   if (x is null) {}
来源：http://zpz.ydzc1.top

[P07] 防抖与节流
来源：http://dae.haohaochexian.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mvp.dianchejie.cn

PHP:  // 手写时间戳比较
来源：http://kbt.havefunace.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cmi.gotoacloud.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ebl.guannengcc.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hyt.cashguo.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nsd.xuetiantiany.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://uah.fengsongda.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qbq.jlsjyb.cn

[P08] 处理浮点精度问题
来源：http://ths.daria6918.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fuq.xingfuxueyuan.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vpx.jqgfzy.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mea.jiagoushi.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tmd.xingfuxueyuan.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://eel.havefunace.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mwy.chenlongwang.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://exx.epnwcf.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rqa.pengpengdd.cyou

================================================================================
来源：http://htp.tianlin.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xdj.andypj.xyz

================================================================================
来源：http://huc.birdmap.top

[Q01] 创建表
来源：http://syc.smart0.xyz

CREATE TABLE users (
来源：http://mls.gotoacloud.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://pfu.cashguo.top

name VARCHAR(50) NOT NULL,
来源：http://xkf.sufxvd.cn

email VARCHAR(100) UNIQUE,
来源：http://lvf.tianlin.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wam.fanxiaobao.xyz

);
来源：http://cjd.ydzc1.top

[Q02] 创建带外键的表
来源：http://tqj.nwbrower.top

CREATE TABLE orders (
来源：http://pkq.jinqigfzy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wjr.xziqi.cn

user_id INT NOT NULL,
来源：http://hld.fehbvm.com

amount DECIMAL(10, 2),
来源：http://ajb.wangshuangyany.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ual.yanxiufei.cn

);
来源：http://apg.vehdjk.com

[Q03] 增加列
来源：http://avk.yj20258.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://oxi.tian-w.cn

[Q04] 修改列类型
来源：http://nqr.52xcode.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xhp.gaohongyu789.top

[Q05] 重命名列
来源：http://iby.ydzc1.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fvn.nanxuanxn.top

[Q06] 删除列
来源：http://xyx.cdnleiting.top

ALTER TABLE users DROP COLUMN age;
来源：http://zal.dianchejie.cn

[Q07] 删除表
来源：http://yhd.yuxming.cn

DROP TABLE IF EXISTS orders;
来源：http://cqm.yuxming.cn

[Q08] 创建普通索引
来源：http://xbf.bbcook.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://zgo.zhijiandao.cn

[Q09] 创建唯一索引
来源：http://awv.birdmap.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://llu.redwolf501.top

[Q10] 插入单行
来源：http://uff.zhoulong.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://cyp.meibo888.top

[Q11] 一次插入多行
来源：http://shw.jlsjyb.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pab.epnwcf.com

[Q12] 插入后取自增 ID
来源：http://olv.ybcxt.top

INSERT INTO users (name) VALUES ('C');
来源：http://mtn.sysykeji.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kph.fanxiaobao.xyz

[Q13] 忽略重复插入
来源：http://qtn.svipenyu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pld.jqgfzy.top

[Q14] 存在则更新（upsert）
来源：http://dht.yj20258888.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vpp.zhengqikj.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://avu.gotoacloud.top

[Q15] 查询全部
来源：http://qxx.zhijiandao.cn

SELECT * FROM users;
来源：http://dml.zhongyouzk.top

[Q16] 查询指定列
来源：http://ksf.xuetiantiany.cn

SELECT id, name FROM users;
来源：http://ipr.yongpay.top

[Q17] 条件查询
来源：http://pmv.jinyuanbaomall.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qir.cdnleiting.top

[Q18] 模糊匹配
来源：http://zqd.chenjidiqi.icu

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kdw.bbcook.cn

[Q19] 范围查询
来源：http://miq.ydjk.org.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nre.guannengcc.top

[Q20] IN 列表
来源：http://adv.sxryk.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ydk.hongshengwenyu.top

[Q21] 空值判断
来源：http://maf.bjfxy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://wst.kuanghao11.cn

[Q22] 排序
来源：http://aba.bbcook.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vas.hysaishi.cn

[Q23] 分页
来源：http://fgj.jinqigufen.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gee.jinqigufen.top

[Q24] 去重
来源：http://keh.hesvh.cn

SELECT DISTINCT city FROM users;
来源：http://hwe.nanxuanxn.top

[Q25] 只取前 N 条
来源：http://zoj.sjlbkw.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fuf.52xcode.cn

[Q26] 计数
来源：http://yrq.zhijiandao.cn

SELECT COUNT(*) FROM users;
来源：http://yfb.wangdashe.top

[Q27] 条件计数
来源：http://ern.jqgfzy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vgg.fengsongda.top

[Q28] 求和与平均
来源：http://voj.yonumen.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ybm.jqgfzy.top

[Q29] 最大最小值
来源：http://kmp.xuetiantiany.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://usn.gogol.net.cn

[Q30] 分组统计
来源：http://hqp.zhongyouzk.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ofm.nanxinkj.top

[Q31] 分组后过滤
来源：http://kal.tian-w.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rqw.hnxiangtu.top

[Q32] 分组拼接字符串
来源：http://qhq.zycfv.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ekq.wangdashe.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ivi.jianghu66.top

[Q33] 多列分组
来源：http://ita.jqgufenzy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vfg.xuetiantiany.cn

[Q34] 每组取第一条
来源：http://bop.yuxming.cn

SELECT * FROM (
来源：http://kms.hywenlv.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cwt.jqgufenzy.top

) t WHERE rn = 1;
来源：http://gsv.aibaodan.cn

[Q35] 内连接
来源：http://uii.shangyingyoupin.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ctm.aizwys.cn

[Q36] 左连接
来源：http://paw.jinyuanbaomall.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fgu.bbcook.cn

[Q37] 右连接
来源：http://fpi.zhixingplan.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jlv.mhx1999.top

[Q38] 全外连接（PostgreSQL）
来源：http://jlt.xuetiantiany.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yyq.yuxming.cn

[Q39] 自连接（查上下级）
来源：http://evm.wangdashe.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://tbb.shanyushiyangtech.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gho.jinqigufen.top

[Q40] 交叉连接（笛卡尔积）
来源：http://mti.cucudq.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://yml.ivvv.top

[Q41] 多表连接
来源：http://kil.vqdsnc.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://bmu.cqqwz.cn

JOIN users u ON u.id = o.user_id
来源：http://enh.fehbvm.com

JOIN products p ON p.id = o.product_id;
来源：http://qxz.wangdashe.top

[Q42] 连接条件附加过滤
来源：http://wha.zdbjq.cn

SELECT u.name, o.amount FROM users u
来源：http://dos.ydzc1.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ldr.jiagoushi.top

[Q43] 标量子查询
来源：http://dlj.c1oappe.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rps.vqdsnc.cn

[Q44] IN 子查询
来源：http://lle.zhengqikj.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kit.xylfe.cn

[Q45] EXISTS 判断存在
来源：http://cia.zhengqikj.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vra.sufxvd.cn

[Q46] NOT EXISTS 判断不存在
来源：http://dyl.zhijiandao.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jdq.ybcxt.top

[Q47] 与平均值比较
来源：http://rev.aibaodan.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jsv.shzxlz.cn

[Q48] CTE 公用表表达式
来源：http://zwo.yj20258.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vkr.birdmap.top

SELECT * FROM t WHERE c > 5;
来源：http://buu.zhixingplan.top

[Q49] 更新单行
来源：http://mjs.jiagoushi.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vwe.nanxuanxn.top

[Q50] 批量更新
来源：http://duo.hfpthk.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dqy.zdbjq.cn

[Q51] 用子查询更新
来源：http://ozs.gzhubu.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rlx.hfpthk.cn

[Q52] 删除指定行
来源：http://kvr.yj20258.top

DELETE FROM users WHERE id = 10;
来源：http://grn.yueranfly.top

[Q53] 按条件删除
来源：http://yxo.jinghuilouyu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yjs.gogol.net.cn

[Q54] 清空表
来源：http://sxf.gogol.net.cn

TRUNCATE TABLE logs;
来源：http://nad.andypj.xyz

[Q55] 排名（并列占位）
来源：http://jgc.meibo888.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dfi.hysaishi.cn

[Q56] 密集排名（并列不占位）
来源：http://xnd.jinyuanbaomall.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://sge.gzhubu.top

[Q57] 行号
来源：http://kvw.hcnkem.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bby.chenzaomai.com

[Q58] 累计求和
来源：http://sgx.chenjidiqi.icu

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://thv.iojbl.cn

[Q59] 分组内累计
来源：http://eud.jqgufenzy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://uwp.tianlin.xyz

[Q60] 取上一行 / 下一行
来源：http://qbn.gogol.net.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rju.0kj1m.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gli.smart0.xyz


<!-- 参考信息 -->
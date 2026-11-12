代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://ubp.daxiang520.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ywv.sufxvd.cn

[N11] 二叉树中序遍历
来源：http://jyk.nanxuanxn.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uth.hywenlv.cn

PHP:  // 手写递归函数
来源：http://icc.tanke756.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vjd.tianlin.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fkg.ywan-chungtsiang.top

Java: // 手写递归
来源：http://sqy.0kj1m.cn

Go:   // 手写递归
来源：http://ofg.kuanghao11.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pwx.ydjk.org.cn

C#:   // 手写递归
来源：http://okw.tian-w.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hzs.hywenlv.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kby.0kj1m.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dia.shangyingyoupin.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rhz.9152youxi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rxy.guowangkeji.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ivg.haohaochexian.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yoa.zhaomingkeji.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bjj.xuanzx.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pgc.sxryk.cn

================================================================================
来源：http://rfo.pycfn.com

O. 并发与异步
来源：http://shk.zdqjudy.top

================================================================================
来源：http://gmo.gzhubu.top

[O01] 启动一个线程
来源：http://qfl.tarul.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hqw.cucudq.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dnh.hfpthk.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bwj.sjlbkw.cn

TS:   // 同 JS
来源：http://nxz.havefunace.top

Java: new Thread(() -> f()).start()
来源：http://hvm.zhoulong.xyz

Go:   go f()
来源：http://wyz.cqqwz.cn

Ruby: Thread.new { f }
来源：http://chv.hesvh.cn

C#:   Task.Run(() => F());
来源：http://dbw.jinqigufen.top

[O02] 使用线程池
来源：http://tjp.xuanzx.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ghe.uphjek.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tyt.jqgfzy.top

JS:   // worker_threads 线程池
来源：http://kcz.sweek.top

TS:   // worker_threads 线程池
来源：http://upx.c1oappe.top

Java: Executors.newFixedThreadPool(4)
来源：http://xng.quarkkingdee.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cmj.xylfe.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nrt.jlsjyb.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qkh.kuanghao11.cn

[O03] 加锁保护共享数据
来源：http://goa.gotoacloud.top

Py:   with lock: shared += 1
来源：http://shn.ivvv.top

PHP:  // 用 flock() 做文件锁
来源：http://xaw.ydzc1.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yaw.redwolf501.top

TS:   // 同 JS
来源：http://sev.sweek.top

Java: synchronized (this) { shared++; }
来源：http://dyo.epnwcf.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wme.shzxlz.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ndv.meibo888.top

C#:   lock (gate) { shared++; }
来源：http://wiz.iojbl.cn

[O04] 定义异步函数并等待
来源：http://ptw.yongpay.top

Py:   async def f():⏎    await g()
来源：http://gkk.sjlbkw.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rjq.smart0.xyz

JS:   async function f() { await g(); }
来源：http://pjr.birdmap.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://pqk.hesvh.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ipa.pengpengdd.cyou

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qrl.xinyue.icu

Ruby: # 用 Fiber 或 async gem
来源：http://jpv.fktsv.cn

C#:   async Task F() { await G(); }
来源：http://kyp.hammf.cn

[O05] 并发执行并等待全部完成
来源：http://knz.sjlbkw.cn

Py:   asyncio.gather(*tasks)
来源：http://ldt.zdbjq.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jnk.jinqigufen.top

JS:   await Promise.all(tasks)
来源：http://mvg.snrcjt.cn

TS:   await Promise.all(tasks)
来源：http://fgz.birdmap.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xgs.zhengqikj.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vyg.cheryme.top

Ruby: threads.map(&:join)
来源：http://jac.jinghuilouyu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ipw.xziqi.cn

[O06] 使用进程池
来源：http://yeg.wangdashe.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://thp.cdnleiting.top

PHP:  // pcntl_fork 或多进程队列
来源：http://kpj.yongpay.top

JS:   // child_process / cluster 模块
来源：http://hce.xziqi.cn

TS:   // child_process / cluster 模块
来源：http://sls.daxiang520.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://moh.xuetiantiany.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wvt.wangshuangyany.cn

Ruby: // fork 块
来源：http://ued.ydjk.org.cn

C#:   Parallel.For
来源：http://por.jinqigufen.top

================================================================================
来源：http://gto.jinghuilouyu.cn

P. 常用工具函数
来源：http://rik.daria6918.cn

================================================================================
来源：http://msp.hnqzz.top

[P01] 生成 UUID
来源：http://tfy.yanxiufei.cn

Py:   str(uuid.uuid4())
来源：http://tiw.jlsjyb.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://geb.zhoulong.xyz

JS:   crypto.randomUUID()
来源：http://hzp.yangfankeji.com

TS:   crypto.randomUUID()
来源：http://tgj.guannengcc.top

Java: UUID.randomUUID().toString()
来源：http://vqr.ppjwa.cn

Go:   // 用 github.com/google/uuid
来源：http://qrw.yj20258888.top

Ruby: SecureRandom.uuid
来源：http://sbp.fzhhl.top

C#:   Guid.NewGuid().ToString()
来源：http://qjk.jinqigfzy.top

[P02] MD5 / SHA256 摘要
来源：http://qdw.zdqjudy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gsl.zdqjudy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://exi.andypj.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kup.cucudq.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bcl.dashuyun.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zff.jlsjyb.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://iea.zhaomingkeji.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://awd.xinyue.icu

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mac.xuanzx.com

[P03] 生成短随机字符串
来源：http://xgb.sxryk.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qqn.iojbl.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xkj.redwolf501.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rst.cucudq.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jgi.nwbrower.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qtz.sysykeji.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yil.9152youxi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ltf.hongshengwenyu.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rql.birdmap.top

[P04] 求长度
来源：http://gjc.zycfv.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://puy.ctjpmb.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zug.zhengqikj.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lnn.jinqigfzy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mnz.kuanghao11.cn

Java: list.size();  map.size();  s.length()
来源：http://pbl.kuanghao11.cn

Go:   len(arr);  len(m)
来源：http://uad.feifeiyinyue.top

Ruby: x.length;  x.size
来源：http://fzs.zhongyouzk.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ruj.sjlbkw.cn

[P05] 判断两个对象内容是否相等
来源：http://xxc.gzhubu.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ccm.ydzc1.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wmu.c1oappe.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mtx.bbcook.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lfm.xuanzx.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ter.jinqigufen.top

Go:   reflect.DeepEqual(a, b)
来源：http://bva.ppjwa.cn

Ruby: a == b
来源：http://fuc.yj20258888.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://oqa.cqqwz.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wgk.snrcjt.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bqy.vehdjk.com

PHP:  if (empty($x)) {}
来源：http://ymw.daxiang520.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ovk.shanyushiyangtech.top

TS:   if (x == null) {}
来源：http://oxd.xingfuxueyuan.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://crr.zhijiandao.cn

Go:   if x == nil {}
来源：http://tqm.fengsongda.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://obk.316326.xyz

C#:   if (x is null) {}
来源：http://vcj.xziqi.cn

[P07] 防抖与节流
来源：http://fdd.aizwys.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tly.9152youxi.cn

PHP:  // 手写时间戳比较
来源：http://yko.pycfn.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tyv.haohaochexian.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wdp.zhongyouzk.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xhu.hfpthk.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ket.jinqigufen.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://aur.fengsongda.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://emv.bbcook.cn

[P08] 处理浮点精度问题
来源：http://usg.dianchejie.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://avh.chenjidiqi.icu

PHP:  bcadd("0.1", "0.2", 2);
来源：http://uly.xylfe.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://oux.zhaomingkeji.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://clo.jqgfzy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ryo.pycfn.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://coe.zhijiandao.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dqi.wangdashe.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tjg.vehdjk.com

================================================================================
来源：http://yfd.tarul.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://atn.meibo888.top

================================================================================
来源：http://hrb.daxiang520.top

[Q01] 创建表
来源：http://nje.yj20258.top

CREATE TABLE users (
来源：http://odc.hongshengwenyu.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vvw.jqgufenzy.top

name VARCHAR(50) NOT NULL,
来源：http://ayu.jqgufenzy.top

email VARCHAR(100) UNIQUE,
来源：http://wec.xinyue.icu

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ymg.shuidangran.top

);
来源：http://mjo.yvedp.cn

[Q02] 创建带外键的表
来源：http://brl.yangfankeji.com

CREATE TABLE orders (
来源：http://dhn.hesvh.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tpc.xylfe.cn

user_id INT NOT NULL,
来源：http://nyd.xuetiantiany.cn

amount DECIMAL(10, 2),
来源：http://upb.zdbjq.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jhk.sufxvd.cn

);
来源：http://cvm.uphjek.com

[Q03] 增加列
来源：http://qdh.hesvh.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://yzx.yanxiufei.cn

[Q04] 修改列类型
来源：http://joi.316326.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kmj.shuidangran.top

[Q05] 重命名列
来源：http://rpk.ivvv.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gzx.ivvv.top

[Q06] 删除列
来源：http://bdw.wangdashe.top

ALTER TABLE users DROP COLUMN age;
来源：http://ire.svipenyu.cn

[Q07] 删除表
来源：http://scj.52xcode.cn

DROP TABLE IF EXISTS orders;
来源：http://uqb.xuetiantiany.cn

[Q08] 创建普通索引
来源：http://cgn.zdbjq.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://taw.birdmap.top

[Q09] 创建唯一索引
来源：http://gdu.uphjek.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zdn.daria6918.cn

[Q10] 插入单行
来源：http://mdi.wangshuangyany.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ybe.cdnleiting.top

[Q11] 一次插入多行
来源：http://pzq.sysykeji.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://moe.hesvh.cn

[Q12] 插入后取自增 ID
来源：http://tmy.yongpay.top

INSERT INTO users (name) VALUES ('C');
来源：http://dfl.bjfxy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qgr.chenjidiqi.icu

[Q13] 忽略重复插入
来源：http://hrg.svipenyu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dwu.zdqjudy.top

[Q14] 存在则更新（upsert）
来源：http://leq.vehdjk.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://lgx.c1oappe.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yap.guowangkeji.top

[Q15] 查询全部
来源：http://fxy.quarkkingdee.top

SELECT * FROM users;
来源：http://wpo.zhijiandao.cn

[Q16] 查询指定列
来源：http://mms.sxryk.cn

SELECT id, name FROM users;
来源：http://uxq.sweek.top

[Q17] 条件查询
来源：http://ofc.shanyushiyangtech.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vhr.xuanzx.com

[Q18] 模糊匹配
来源：http://pph.yuxming.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mot.wangshuangyany.cn

[Q19] 范围查询
来源：http://dfb.zhoulong.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://oaf.zhongyouzk.top

[Q20] IN 列表
来源：http://jca.xziqi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tro.yuanzhike.top

[Q21] 空值判断
来源：http://lwk.sweek.top

SELECT * FROM users WHERE email IS NULL;
来源：http://aly.yvedp.cn

[Q22] 排序
来源：http://cza.0kj1m.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dds.bjfxy.top

[Q23] 分页
来源：http://guy.hnqzz.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gvv.fzhhl.top

[Q24] 去重
来源：http://jlg.nanxuanxn.top

SELECT DISTINCT city FROM users;
来源：http://nxy.jqgfzy.top

[Q25] 只取前 N 条
来源：http://bka.bjfxy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://olo.sxryk.cn

[Q26] 计数
来源：http://des.shanyushiyangkeji.top

SELECT COUNT(*) FROM users;
来源：http://pbv.jianghu66.top

[Q27] 条件计数
来源：http://hfi.guannengcc.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qoi.cheryme.top

[Q28] 求和与平均
来源：http://mgv.tianlin.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ekh.jianghu66.top

[Q29] 最大最小值
来源：http://wgl.zhengqikj.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ymr.tianlin.xyz

[Q30] 分组统计
来源：http://uyj.zhiwuduotai.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ueu.smart0.xyz

[Q31] 分组后过滤
来源：http://ppo.xuetiantiany.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qkt.pycfn.com

[Q32] 分组拼接字符串
来源：http://itz.uphjek.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tph.hywenlv.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ilc.gotoacloud.top

[Q33] 多列分组
来源：http://bav.nanxuanxn.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pgt.xinyue.icu

[Q34] 每组取第一条
来源：http://wlr.yuxming.cn

SELECT * FROM (
来源：http://ymq.jiagoushi.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://coy.iojbl.cn

) t WHERE rn = 1;
来源：http://neg.shanyushiyangtech.top

[Q35] 内连接
来源：http://mrn.fktsv.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fae.hywenlv.cn

[Q36] 左连接
来源：http://hwt.gogol.net.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cey.yj202588.top

[Q37] 右连接
来源：http://wkk.jyoumei.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zvy.meibo888.top

[Q38] 全外连接（PostgreSQL）
来源：http://ozy.mhx1999.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://php.quarkkingdee.top

[Q39] 自连接（查上下级）
来源：http://aim.redwolf501.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://cri.daria6918.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://sml.gotoacloud.top

[Q40] 交叉连接（笛卡尔积）
来源：http://rxz.fzhhl.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://her.sufxvd.cn

[Q41] 多表连接
来源：http://jkj.ivvv.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://zes.zhaomingkeji.xyz

JOIN users u ON u.id = o.user_id
来源：http://cgn.yj202588.top

JOIN products p ON p.id = o.product_id;
来源：http://tll.c1oappe.top

[Q42] 连接条件附加过滤
来源：http://mxn.jianghu66.top

SELECT u.name, o.amount FROM users u
来源：http://xrl.mhx1999.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qru.tanke756.top

[Q43] 标量子查询
来源：http://pqx.zhijiandao.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://toj.jinghuilouyu.cn

[Q44] IN 子查询
来源：http://olb.zhixingplan.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://noc.birdmap.top

[Q45] EXISTS 判断存在
来源：http://mqt.yj20258888.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rtv.yongpay.top

[Q46] NOT EXISTS 判断不存在
来源：http://hya.zhiwuduotai.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://giu.sweek.top

[Q47] 与平均值比较
来源：http://wwg.ehwqpu.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lwl.haohaochexian.top

[Q48] CTE 公用表表达式
来源：http://flr.gotoacloud.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pye.ppjwa.cn

SELECT * FROM t WHERE c > 5;
来源：http://gbk.nanxuanxn.top

[Q49] 更新单行
来源：http://ril.vqdsnc.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xtn.gogol.net.cn

[Q50] 批量更新
来源：http://mug.yj202588.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qgy.shanyushiyangkeji.top

[Q51] 用子查询更新
来源：http://arg.chenjidiqi.icu

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wjl.52xcode.cn

[Q52] 删除指定行
来源：http://umk.yuxming.cn

DELETE FROM users WHERE id = 10;
来源：http://vwq.gotoacloud.top

[Q53] 按条件删除
来源：http://dwv.ydzc1.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://cvt.zycfv.cn

[Q54] 清空表
来源：http://ksy.xziqi.cn

TRUNCATE TABLE logs;
来源：http://liz.xziqi.cn

[Q55] 排名（并列占位）
来源：http://hpc.nwbrower.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://sjk.jinghuilouyu.cn

[Q56] 密集排名（并列不占位）
来源：http://oqd.sysykeji.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://imy.jinqigfzy.top

[Q57] 行号
来源：http://izx.c1oappe.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ncz.shanyushiyangtech.top

[Q58] 累计求和
来源：http://siu.jyoumei.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://olk.kuanghao11.cn

[Q59] 分组内累计
来源：http://hkz.sxryk.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mng.yj20258888.top

[Q60] 取上一行 / 下一行
来源：http://vzp.havefunace.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kwh.hnqzz.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vgv.ybcxt.top

[Q61] 移动平均
来源：http://uoc.ivvv.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nqc.snrcjt.cn

[Q62] 分组占比
来源：http://dfz.shangyingyoupin.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mql.snrcjt.cn


<!-- 参考信息 -->
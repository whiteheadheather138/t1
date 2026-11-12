代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://ucp.hfpthk.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://vla.cdnleiting.top

[N11] 二叉树中序遍历
来源：http://iuh.316326.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lyk.hnxiangtu.top

PHP:  // 手写递归函数
来源：http://nll.yfazqb.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ifq.birdmap.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zky.zhaomingkeji.xyz

Java: // 手写递归
来源：http://bjh.xinyue.icu

Go:   // 手写递归
来源：http://pdi.ehwqpu.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gbp.tanke756.top

C#:   // 手写递归
来源：http://axn.chenlongwang.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xlj.dianchejie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ujl.xziqi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cto.birdmap.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://arh.xziqi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pcv.cdnleiting.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lgf.feifeiyinyue.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kfx.hysaishi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://arr.pengpengdd.cyou

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vft.ybcxt.top

================================================================================
来源：http://wyg.sxryk.cn

O. 并发与异步
来源：http://orw.daxiang520.top

================================================================================
来源：http://rne.hywenlv.cn

[O01] 启动一个线程
来源：http://jof.hnqzz.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rhv.dashuyun.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kla.jqgufenzy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wtk.fengsongda.top

TS:   // 同 JS
来源：http://pfp.yfazqb.com

Java: new Thread(() -> f()).start()
来源：http://nhd.hesvh.cn

Go:   go f()
来源：http://rhd.pengpengdd.cyou

Ruby: Thread.new { f }
来源：http://gqj.ehwqpu.com

C#:   Task.Run(() => F());
来源：http://avr.shangyingyoupin.top

[O02] 使用线程池
来源：http://vyb.zhiwuduotai.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wbb.hammf.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nev.52xcode.cn

JS:   // worker_threads 线程池
来源：http://iyq.ywan-chungtsiang.top

TS:   // worker_threads 线程池
来源：http://dii.jlsjyb.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ruz.iojbl.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ahw.chenlongwang.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rdu.gzhubu.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wqm.kuanghao11.cn

[O03] 加锁保护共享数据
来源：http://obo.ivvv.top

Py:   with lock: shared += 1
来源：http://dwj.hammf.cn

PHP:  // 用 flock() 做文件锁
来源：http://ply.zycfv.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fma.yuxming.cn

TS:   // 同 JS
来源：http://tyr.zhongyouzk.top

Java: synchronized (this) { shared++; }
来源：http://ihr.gotoacloud.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gfj.wangdashe.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://fmm.wangdashe.top

C#:   lock (gate) { shared++; }
来源：http://pqd.shanyushiyangtech.top

[O04] 定义异步函数并等待
来源：http://eex.yanxiufei.cn

Py:   async def f():⏎    await g()
来源：http://ild.birdmap.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://int.hnqzz.top

JS:   async function f() { await g(); }
来源：http://bmm.hongshengwenyu.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://var.uphjek.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://aew.nanxuanxn.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wsi.0kj1m.cn

Ruby: # 用 Fiber 或 async gem
来源：http://dmw.havefunace.top

C#:   async Task F() { await G(); }
来源：http://nsk.chenzaomai.com

[O05] 并发执行并等待全部完成
来源：http://fch.haohaochexian.top

Py:   asyncio.gather(*tasks)
来源：http://wpe.redwolf501.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fzw.jqgufenzy.top

JS:   await Promise.all(tasks)
来源：http://nrx.xingfuxueyuan.xyz

TS:   await Promise.all(tasks)
来源：http://dss.yj20258888.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rbv.zhongyouzk.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bqo.cashguo.top

Ruby: threads.map(&:join)
来源：http://mzo.zdbjq.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://vue.ehwqpu.com

[O06] 使用进程池
来源：http://tce.hysaishi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kkn.nanxuanxn.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ayl.yj20258888.top

JS:   // child_process / cluster 模块
来源：http://djw.jinqigfzy.top

TS:   // child_process / cluster 模块
来源：http://mpb.chenjidiqi.icu

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jed.kuanghao11.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zlh.pycfn.com

Ruby: // fork 块
来源：http://uwl.jinqigufen.top

C#:   Parallel.For
来源：http://uhp.andypj.xyz

================================================================================
来源：http://cvy.zdbjq.cn

P. 常用工具函数
来源：http://imf.svipenyu.cn

================================================================================
来源：http://yub.nanxinkj.top

[P01] 生成 UUID
来源：http://nko.xingfuxueyuan.xyz

Py:   str(uuid.uuid4())
来源：http://zzg.gaohongyu789.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dwf.chenzaomai.com

JS:   crypto.randomUUID()
来源：http://ihj.aibaodan.cn

TS:   crypto.randomUUID()
来源：http://gat.gogol.net.cn

Java: UUID.randomUUID().toString()
来源：http://sht.ydjk.org.cn

Go:   // 用 github.com/google/uuid
来源：http://zaq.jlsjyb.cn

Ruby: SecureRandom.uuid
来源：http://feu.xylfe.cn

C#:   Guid.NewGuid().ToString()
来源：http://ezi.jinyuanbaomall.cn

[P02] MD5 / SHA256 摘要
来源：http://iud.xinyue.icu

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nxf.hnxiangtu.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://fpn.jqgfzy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xnm.shanyushiyangkeji.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ixv.sjlbkw.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://puq.cucudq.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://oow.xuanzx.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vzl.wangdashe.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://eje.gotoacloud.top

[P03] 生成短随机字符串
来源：http://zxd.shzxlz.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qsv.mhx1999.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pcl.jqgfzy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zim.nanxinkj.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rxr.feifeiyinyue.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tbv.sufxvd.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jys.haohaochexian.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://seh.meibo888.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mds.sjlbkw.cn

[P04] 求长度
来源：http://rdm.wangdashe.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://riz.redwolf501.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ihg.gogol.net.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uxb.zhoulong.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pra.ydjk.org.cn

Java: list.size();  map.size();  s.length()
来源：http://pnv.cdnleiting.top

Go:   len(arr);  len(m)
来源：http://lpq.xylfe.cn

Ruby: x.length;  x.size
来源：http://vhd.ppjwa.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://svz.zhiwuduotai.top

[P05] 判断两个对象内容是否相等
来源：http://hns.nanxinkj.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://kpo.chenlongwang.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nqw.jinyuanbaomall.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pts.yj20258.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ahl.shzxlz.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://arl.sufxvd.cn

Go:   reflect.DeepEqual(a, b)
来源：http://dms.fehbvm.com

Ruby: a == b
来源：http://zem.chenlongwang.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ngu.yueranfly.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pip.wangshuangyany.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://aeo.gzhubu.top

PHP:  if (empty($x)) {}
来源：http://ypd.shzxlz.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wxz.shangyingyoupin.top

TS:   if (x == null) {}
来源：http://pyq.ctjpmb.com

Java: if (x == null || x.isEmpty()) {}
来源：http://cvs.dashuyun.cn

Go:   if x == nil {}
来源：http://boa.andypj.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://avq.cqqwz.cn

C#:   if (x is null) {}
来源：http://pdo.daxiang520.top

[P07] 防抖与节流
来源：http://dai.aizwys.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kjc.ybcxt.top

PHP:  // 手写时间戳比较
来源：http://bik.hysaishi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bbs.andypj.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hcl.yueranfly.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zcw.fehbvm.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mwe.zdbjq.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ies.ydjk.org.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vnv.hesvh.cn

[P08] 处理浮点精度问题
来源：http://cfy.smart0.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://yui.zhixingplan.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://oiy.shanyushiyangtech.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yxr.sxryk.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ddv.ybcxt.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zlc.xingfuxueyuan.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://otz.jqgufenzy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tnb.nanxuanxn.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hsd.shanyushiyangkeji.top

================================================================================
来源：http://qpw.andypj.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cla.yueranfly.top

================================================================================
来源：http://qvw.yj20258.top

[Q01] 创建表
来源：http://glt.bjfxy.top

CREATE TABLE users (
来源：http://bwz.svipenyu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bmk.gaohongyu789.top

name VARCHAR(50) NOT NULL,
来源：http://tfm.svipenyu.cn

email VARCHAR(100) UNIQUE,
来源：http://iij.yonumen.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://txc.0kj1m.cn

);
来源：http://gwa.zhongyouzk.top

[Q02] 创建带外键的表
来源：http://rhp.xuanzx.com

CREATE TABLE orders (
来源：http://hbp.redwolf501.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vcf.dashuyun.cn

user_id INT NOT NULL,
来源：http://znl.yueranfly.top

amount DECIMAL(10, 2),
来源：http://enb.kuanghao11.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://roj.sjlbkw.cn

);
来源：http://vvp.0kj1m.cn

[Q03] 增加列
来源：http://stx.yfazqb.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rxb.sysykeji.top

[Q04] 修改列类型
来源：http://wro.xuetiantiany.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dqm.hongshengwenyu.top

[Q05] 重命名列
来源：http://jyq.feifeiyinyue.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tnw.shangyingyoupin.top

[Q06] 删除列
来源：http://aqo.yangfankeji.com

ALTER TABLE users DROP COLUMN age;
来源：http://zzs.andypj.xyz

[Q07] 删除表
来源：http://pqp.aibaodan.cn

DROP TABLE IF EXISTS orders;
来源：http://ymu.zdbjq.cn

[Q08] 创建普通索引
来源：http://jxk.jinyuanbaomall.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://qaz.shangyingyoupin.top

[Q09] 创建唯一索引
来源：http://jqf.cdnleiting.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dym.zhijiandao.cn

[Q10] 插入单行
来源：http://ckp.guowangkeji.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wod.mhx1999.top

[Q11] 一次插入多行
来源：http://tio.guannengcc.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ryn.0kj1m.cn

[Q12] 插入后取自增 ID
来源：http://yxr.shzxlz.cn

INSERT INTO users (name) VALUES ('C');
来源：http://cbt.jianghu66.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ypx.zycfv.cn

[Q13] 忽略重复插入
来源：http://dcl.shangyingyoupin.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://max.zhongyouzk.top

[Q14] 存在则更新（upsert）
来源：http://wos.bjfxy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jef.zhongyouzk.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pst.shanyushiyangtech.top

[Q15] 查询全部
来源：http://wie.kuanghao11.cn

SELECT * FROM users;
来源：http://eaw.gotoacloud.top

[Q16] 查询指定列
来源：http://zxl.pycfn.com

SELECT id, name FROM users;
来源：http://wzg.yvedp.cn

[Q17] 条件查询
来源：http://rrg.dianchejie.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://men.dashuyun.cn

[Q18] 模糊匹配
来源：http://ovq.ehwqpu.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lwb.xylfe.cn

[Q19] 范围查询
来源：http://jvb.jqgufenzy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wvl.zhoulong.xyz

[Q20] IN 列表
来源：http://att.fehbvm.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pou.ctjpmb.com

[Q21] 空值判断
来源：http://njt.aibaodan.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://nsn.nanxuanxn.top

[Q22] 排序
来源：http://xxn.tarul.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wbe.shuidangran.top

[Q23] 分页
来源：http://xhn.xuanzx.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wcq.cqqwz.cn

[Q24] 去重
来源：http://dbh.hysaishi.cn

SELECT DISTINCT city FROM users;
来源：http://wxl.fktsv.cn

[Q25] 只取前 N 条
来源：http://oqy.zhoulong.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gqr.jqgufenzy.top

[Q26] 计数
来源：http://eed.wangdashe.top

SELECT COUNT(*) FROM users;
来源：http://wcb.daxiang520.top

[Q27] 条件计数
来源：http://nbe.zhijiandao.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nof.hywenlv.cn

[Q28] 求和与平均
来源：http://ocb.zhaomingkeji.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vfe.jinqigfzy.top

[Q29] 最大最小值
来源：http://vqm.sjlbkw.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://pxf.daxiang520.top

[Q30] 分组统计
来源：http://ntg.xylfe.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://crk.ehwqpu.com

[Q31] 分组后过滤
来源：http://qpa.zhixingplan.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://tct.hywenlv.cn

[Q32] 分组拼接字符串
来源：http://ctw.nanxinkj.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jhj.yuxming.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://upo.gzhubu.top

[Q33] 多列分组
来源：http://zmm.hnxiangtu.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cxv.fzhhl.top

[Q34] 每组取第一条
来源：http://xak.redwolf501.top

SELECT * FROM (
来源：http://ykj.sweek.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pkw.hongshengwenyu.top

) t WHERE rn = 1;
来源：http://axf.zdqjudy.top

[Q35] 内连接
来源：http://zyj.zhixingplan.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://arz.jinqigufen.top

[Q36] 左连接
来源：http://aah.yueranfly.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gft.mhx1999.top

[Q37] 右连接
来源：http://ysq.gaohongyu789.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ssl.c1oappe.top

[Q38] 全外连接（PostgreSQL）
来源：http://qdr.jinqigfzy.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gdf.cashguo.top

[Q39] 自连接（查上下级）
来源：http://prz.andypj.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://chk.uphjek.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://sje.sjlbkw.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://jjy.sxryk.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hui.daxiang520.top

[Q41] 多表连接
来源：http://rhr.fzhhl.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://fli.yj20258.top

JOIN users u ON u.id = o.user_id
来源：http://tos.fzhhl.top

JOIN products p ON p.id = o.product_id;
来源：http://bst.ppjwa.cn

[Q42] 连接条件附加过滤
来源：http://tkp.zdbjq.cn

SELECT u.name, o.amount FROM users u
来源：http://swh.sufxvd.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://eok.yonumen.top

[Q43] 标量子查询
来源：http://mqu.hysaishi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ddc.shanyushiyangtech.top

[Q44] IN 子查询
来源：http://mmx.pengpengdd.cyou

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vce.316326.xyz

[Q45] EXISTS 判断存在
来源：http://gap.dashuyun.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kmt.zhijiandao.cn

[Q46] NOT EXISTS 判断不存在
来源：http://hce.nanxuanxn.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rbo.jianghu66.top

[Q47] 与平均值比较
来源：http://yth.bbcook.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ysf.hammf.cn

[Q48] CTE 公用表表达式
来源：http://kzu.zhixingplan.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://aai.jqgfzy.top

SELECT * FROM t WHERE c > 5;
来源：http://zrl.hongshengwenyu.top

[Q49] 更新单行
来源：http://apt.dianchejie.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tbs.yuanzhike.top

[Q50] 批量更新
来源：http://hgj.aizwys.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dzh.jyoumei.cn

[Q51] 用子查询更新
来源：http://bww.aibaodan.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://nfa.aizwys.cn

[Q52] 删除指定行
来源：http://nmg.yueranfly.top

DELETE FROM users WHERE id = 10;
来源：http://bjd.shanyushiyangkeji.top

[Q53] 按条件删除
来源：http://hiv.pengpengdd.cyou

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tol.yfazqb.com

[Q54] 清空表
来源：http://qoh.ppjwa.cn

TRUNCATE TABLE logs;
来源：http://edn.nanxinkj.top

[Q55] 排名（并列占位）
来源：http://asm.bjfxy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tfr.guannengcc.top

[Q56] 密集排名（并列不占位）
来源：http://khy.svipenyu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vuq.jinyuanbaomall.cn

[Q57] 行号
来源：http://xgr.zhoulong.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hok.tanke756.top

[Q58] 累计求和
来源：http://eig.jqgufenzy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://uor.yfazqb.com

[Q59] 分组内累计
来源：http://dfm.9152youxi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fbn.xingfuxueyuan.xyz

[Q60] 取上一行 / 下一行
来源：http://uyt.0kj1m.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ghx.dashuyun.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ycb.sxryk.cn

[Q61] 移动平均
来源：http://fih.gotoacloud.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://edj.0kj1m.cn

[Q62] 分组占比
来源：http://rcp.yongpay.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jit.hesvh.cn


<!-- 参考信息 -->
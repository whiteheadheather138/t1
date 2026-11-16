代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://ejn.xuanzx.com

C#:   class Node { public int V; public Node? Next; }
来源：http://eoi.yueranfly.top

[N11] 二叉树中序遍历
来源：http://tuw.fzhhl.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vor.fengsongda.top

PHP:  // 手写递归函数
来源：http://gyk.zhiwuduotai.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pku.ehwqpu.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gni.shanyushiyangkeji.top

Java: // 手写递归
来源：http://jkd.redwolf501.top

Go:   // 手写递归
来源：http://orq.xylfe.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ptz.jinyuanbaomall.cn

C#:   // 手写递归
来源：http://kwk.cashguo.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vdc.chenjidiqi.icu

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bcr.hnqzz.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fqk.yuxming.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sku.zdbjq.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lbb.yonumen.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zil.ywan-chungtsiang.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://htu.guowangkeji.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://agh.vqdsnc.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hlg.xylfe.cn

================================================================================
来源：http://rna.ehwqpu.com

O. 并发与异步
来源：http://dxh.fktsv.cn

================================================================================
来源：http://lvr.ydzc1.top

[O01] 启动一个线程
来源：http://khl.yuxming.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://byd.zhixingplan.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://keq.jqgfzy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fwb.kuanghao11.cn

TS:   // 同 JS
来源：http://exv.nanxuanxn.top

Java: new Thread(() -> f()).start()
来源：http://pal.tanke756.top

Go:   go f()
来源：http://nnr.sysykeji.top

Ruby: Thread.new { f }
来源：http://bnp.jinghuilouyu.cn

C#:   Task.Run(() => F());
来源：http://fis.zhengqikj.top

[O02] 使用线程池
来源：http://edu.ivvv.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yry.hnqzz.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://spa.uphjek.com

JS:   // worker_threads 线程池
来源：http://dkg.daria6918.cn

TS:   // worker_threads 线程池
来源：http://fwm.andypj.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://nga.yfazqb.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://uwe.yuanzhike.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qbf.chenjidiqi.icu

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jfe.yongpay.top

[O03] 加锁保护共享数据
来源：http://ayo.ydjk.org.cn

Py:   with lock: shared += 1
来源：http://yjh.wangdashe.top

PHP:  // 用 flock() 做文件锁
来源：http://nkw.cashguo.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fof.zhijiandao.cn

TS:   // 同 JS
来源：http://way.xziqi.cn

Java: synchronized (this) { shared++; }
来源：http://khu.wangshuangyany.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gnm.zhixingplan.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://fmj.yueranfly.top

C#:   lock (gate) { shared++; }
来源：http://bbm.zhaomingkeji.xyz

[O04] 定义异步函数并等待
来源：http://vrd.wangdashe.top

Py:   async def f():⏎    await g()
来源：http://osl.ctjpmb.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rcb.uphjek.com

JS:   async function f() { await g(); }
来源：http://kdu.chenzaomai.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://yph.epnwcf.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://map.yj20258.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nxo.bjfxy.top

Ruby: # 用 Fiber 或 async gem
来源：http://cji.cdnleiting.top

C#:   async Task F() { await G(); }
来源：http://vsl.feifeiyinyue.top

[O05] 并发执行并等待全部完成
来源：http://oja.zhiwuduotai.top

Py:   asyncio.gather(*tasks)
来源：http://tsb.fehbvm.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zmo.snrcjt.cn

JS:   await Promise.all(tasks)
来源：http://hby.hnqzz.top

TS:   await Promise.all(tasks)
来源：http://gft.yvedp.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jvh.shzxlz.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fmo.zhiwuduotai.top

Ruby: threads.map(&:join)
来源：http://yua.sjlbkw.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://hwh.pengpengdd.cyou

[O06] 使用进程池
来源：http://qot.yuxming.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ifr.tian-w.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://hrh.chenjidiqi.icu

JS:   // child_process / cluster 模块
来源：http://saz.dashuyun.cn

TS:   // child_process / cluster 模块
来源：http://jlo.aibaodan.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tji.fehbvm.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vki.wangdashe.top

Ruby: // fork 块
来源：http://alp.guowangkeji.top

C#:   Parallel.For
来源：http://pwy.bbcook.cn

================================================================================
来源：http://zuy.jinyuanbaomall.cn

P. 常用工具函数
来源：http://nkn.ctjpmb.com

================================================================================
来源：http://has.zdqjudy.top

[P01] 生成 UUID
来源：http://bzw.shzxlz.cn

Py:   str(uuid.uuid4())
来源：http://jit.chenjidiqi.icu

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://uyg.birdmap.top

JS:   crypto.randomUUID()
来源：http://jlu.kuanghao11.cn

TS:   crypto.randomUUID()
来源：http://usa.cheryme.top

Java: UUID.randomUUID().toString()
来源：http://lrt.zycfv.cn

Go:   // 用 github.com/google/uuid
来源：http://sag.bjfxy.top

Ruby: SecureRandom.uuid
来源：http://aur.kuanghao11.cn

C#:   Guid.NewGuid().ToString()
来源：http://san.meibo888.top

[P02] MD5 / SHA256 摘要
来源：http://xeg.gaohongyu789.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zea.aizwys.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://jqr.bjfxy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vrw.yvedp.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jaa.xuanzx.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xmr.hysaishi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kor.jinyuanbaomall.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://alv.tian-w.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kch.hnxiangtu.top

[P03] 生成短随机字符串
来源：http://vzj.cucudq.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://iar.fengsongda.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://izj.dashuyun.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://orh.jqgfzy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ghw.xingfuxueyuan.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zlv.hfpthk.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fey.guowangkeji.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://nhl.uphjek.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ash.nwbrower.top

[P04] 求长度
来源：http://hdt.chenlongwang.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yll.xziqi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ypm.jlsjyb.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lat.snrcjt.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sfh.ydjk.org.cn

Java: list.size();  map.size();  s.length()
来源：http://srq.cashguo.top

Go:   len(arr);  len(m)
来源：http://xls.svipenyu.cn

Ruby: x.length;  x.size
来源：http://awg.bbcook.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://uok.wangshuangyany.cn

[P05] 判断两个对象内容是否相等
来源：http://dct.hcnkem.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://ybq.feifeiyinyue.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ezr.zhiwuduotai.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hdk.yuanzhike.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://itz.tarul.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://uap.iojbl.cn

Go:   reflect.DeepEqual(a, b)
来源：http://rgc.shangyingyoupin.top

Ruby: a == b
来源：http://yfl.zhijiandao.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://uwl.zhoulong.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gwc.jinqigfzy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://prc.yongpay.top

PHP:  if (empty($x)) {}
来源：http://jpd.ctjpmb.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hrj.hesvh.cn

TS:   if (x == null) {}
来源：http://jad.zhongyouzk.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ubp.dashuyun.cn

Go:   if x == nil {}
来源：http://xqz.zhiwuduotai.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://amg.svipenyu.cn

C#:   if (x is null) {}
来源：http://avf.yueranfly.top

[P07] 防抖与节流
来源：http://omf.xinyue.icu

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dro.fengsongda.top

PHP:  // 手写时间戳比较
来源：http://bpi.jinghuilouyu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dwx.zhaomingkeji.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xuw.xylfe.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pgj.hysaishi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kzt.wangdashe.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ciu.zhijiandao.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://elu.yuxming.cn

[P08] 处理浮点精度问题
来源：http://vks.guowangkeji.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ney.ydzc1.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jnc.hfpthk.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://isl.yj202588.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://uxl.shanyushiyangtech.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://khh.yueranfly.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://snz.fzhhl.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://aar.vqdsnc.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ngb.ywan-chungtsiang.top

================================================================================
来源：http://ubd.yuanzhike.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xfy.hongshengwenyu.top

================================================================================
来源：http://wwd.shangyingyoupin.top

[Q01] 创建表
来源：http://pxq.nanxuanxn.top

CREATE TABLE users (
来源：http://fuf.cdnleiting.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mkh.jianghu66.top

name VARCHAR(50) NOT NULL,
来源：http://kbm.guannengcc.top

email VARCHAR(100) UNIQUE,
来源：http://qjo.meibo888.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qwe.fzhhl.top

);
来源：http://bnh.chenjidiqi.icu

[Q02] 创建带外键的表
来源：http://vus.quarkkingdee.top

CREATE TABLE orders (
来源：http://scy.guowangkeji.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nbh.sufxvd.cn

user_id INT NOT NULL,
来源：http://qev.snrcjt.cn

amount DECIMAL(10, 2),
来源：http://wvo.hongshengwenyu.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xrt.andypj.xyz

);
来源：http://edm.jqgufenzy.top

[Q03] 增加列
来源：http://jbc.shanyushiyangtech.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://yrp.guowangkeji.top

[Q04] 修改列类型
来源：http://pdd.hywenlv.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gzh.c1oappe.top

[Q05] 重命名列
来源：http://sih.yj20258.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fuj.pycfn.com

[Q06] 删除列
来源：http://bfj.iojbl.cn

ALTER TABLE users DROP COLUMN age;
来源：http://hch.ywan-chungtsiang.top

[Q07] 删除表
来源：http://giu.yj20258.top

DROP TABLE IF EXISTS orders;
来源：http://jza.jqgfzy.top

[Q08] 创建普通索引
来源：http://nnm.gogol.net.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ebs.yanxiufei.cn

[Q09] 创建唯一索引
来源：http://wdc.gaohongyu789.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qvz.fanxiaobao.xyz

[Q10] 插入单行
来源：http://uxi.xingfuxueyuan.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lwn.zycfv.cn

[Q11] 一次插入多行
来源：http://qfo.fanxiaobao.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kha.bbcook.cn

[Q12] 插入后取自增 ID
来源：http://zql.hammf.cn

INSERT INTO users (name) VALUES ('C');
来源：http://rws.xuanzx.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tuo.xuanzx.com

[Q13] 忽略重复插入
来源：http://iir.gogol.net.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://roq.bjfxy.top

[Q14] 存在则更新（upsert）
来源：http://ntc.hcnkem.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wrl.andypj.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://tns.cucudq.cn

[Q15] 查询全部
来源：http://qvh.xingfuxueyuan.xyz

SELECT * FROM users;
来源：http://xhr.52xcode.cn

[Q16] 查询指定列
来源：http://qjl.bbcook.cn

SELECT id, name FROM users;
来源：http://lem.wangdashe.top

[Q17] 条件查询
来源：http://hoe.hcnkem.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fuy.quarkkingdee.top

[Q18] 模糊匹配
来源：http://hpq.hnqzz.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kmc.quarkkingdee.top

[Q19] 范围查询
来源：http://tkw.jinqigufen.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qrw.shanyushiyangtech.top

[Q20] IN 列表
来源：http://rhh.tarul.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tgu.fktsv.cn

[Q21] 空值判断
来源：http://gwq.jqgfzy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://aqe.hongshengwenyu.top

[Q22] 排序
来源：http://fic.nanxinkj.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nwi.jinyuanbaomall.cn

[Q23] 分页
来源：http://ptv.ybcxt.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://uqu.fanxiaobao.xyz

[Q24] 去重
来源：http://zgy.9152youxi.cn

SELECT DISTINCT city FROM users;
来源：http://qvo.gaohongyu789.top

[Q25] 只取前 N 条
来源：http://sww.pengpengdd.cyou

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mas.sxryk.cn

[Q26] 计数
来源：http://miz.zhaomingkeji.xyz

SELECT COUNT(*) FROM users;
来源：http://poh.jinghuilouyu.cn

[Q27] 条件计数
来源：http://nsq.ybcxt.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tbd.redwolf501.top

[Q28] 求和与平均
来源：http://poc.ivvv.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dme.shanyushiyangtech.top

[Q29] 最大最小值
来源：http://nfr.0kj1m.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://rcg.shuidangran.top

[Q30] 分组统计
来源：http://wnk.hesvh.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gso.havefunace.top

[Q31] 分组后过滤
来源：http://fjz.hcnkem.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fyy.pycfn.com

[Q32] 分组拼接字符串
来源：http://axv.aizwys.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vcj.tanke756.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qxw.pycfn.com

[Q33] 多列分组
来源：http://alu.meibo888.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://nzb.iojbl.cn

[Q34] 每组取第一条
来源：http://qxd.wangdashe.top

SELECT * FROM (
来源：http://xon.shzxlz.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xue.dashuyun.cn

) t WHERE rn = 1;
来源：http://yvo.dianchejie.cn

[Q35] 内连接
来源：http://yqo.yuanzhike.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://iqn.pycfn.com

[Q36] 左连接
来源：http://xtr.yvedp.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dao.jinqigufen.top

[Q37] 右连接
来源：http://obm.jqgufenzy.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://llt.yj20258.top

[Q38] 全外连接（PostgreSQL）
来源：http://mwz.yfazqb.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://sta.dashuyun.cn

[Q39] 自连接（查上下级）
来源：http://qfo.zhijiandao.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://qyw.yvedp.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fkj.zycfv.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://mci.zhixingplan.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://cnf.tanke756.top

[Q41] 多表连接
来源：http://cml.0kj1m.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://kai.sufxvd.cn

JOIN users u ON u.id = o.user_id
来源：http://mou.jlsjyb.cn

JOIN products p ON p.id = o.product_id;
来源：http://dhy.xziqi.cn

[Q42] 连接条件附加过滤
来源：http://gae.feifeiyinyue.top

SELECT u.name, o.amount FROM users u
来源：http://iem.tarul.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mwo.fzhhl.top

[Q43] 标量子查询
来源：http://afl.52xcode.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lwq.zhiwuduotai.top

[Q44] IN 子查询
来源：http://dmf.vqdsnc.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mjf.wangdashe.top

[Q45] EXISTS 判断存在
来源：http://bqj.yueranfly.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qsr.bbcook.cn

[Q46] NOT EXISTS 判断不存在
来源：http://izd.jinqigfzy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uux.jinghuilouyu.cn

[Q47] 与平均值比较
来源：http://ski.hnxiangtu.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zcl.yj20258888.top

[Q48] CTE 公用表表达式
来源：http://axy.hcnkem.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://piu.yonumen.top

SELECT * FROM t WHERE c > 5;
来源：http://jgn.ivvv.top

[Q49] 更新单行
来源：http://tpb.zdqjudy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cpo.andypj.xyz

[Q50] 批量更新
来源：http://rmw.sjlbkw.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zwv.316326.xyz

[Q51] 用子查询更新
来源：http://frd.guowangkeji.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wkr.xziqi.cn

[Q52] 删除指定行
来源：http://miv.zhiwuduotai.top

DELETE FROM users WHERE id = 10;
来源：http://qpt.ydzc1.top

[Q53] 按条件删除
来源：http://mzz.cashguo.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zqm.guowangkeji.top

[Q54] 清空表
来源：http://uvw.feifeiyinyue.top

TRUNCATE TABLE logs;
来源：http://kkr.shzxlz.cn

[Q55] 排名（并列占位）
来源：http://ven.shzxlz.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lre.chenlongwang.top

[Q56] 密集排名（并列不占位）
来源：http://zzm.zhoulong.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ptu.shangyingyoupin.top

[Q57] 行号
来源：http://far.quarkkingdee.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tdq.cqqwz.cn

[Q58] 累计求和
来源：http://zhx.cqqwz.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vhb.yfazqb.com

[Q59] 分组内累计
来源：http://ysx.zhoulong.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fca.pengpengdd.cyou

[Q60] 取上一行 / 下一行
来源：http://yjn.jqgfzy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fhz.havefunace.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jry.xziqi.cn

[Q61] 移动平均
来源：http://zyi.jlsjyb.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bux.jqgfzy.top

[Q62] 分组占比
来源：http://vbp.tarul.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qzt.hnqzz.top


<!-- 参考信息 -->
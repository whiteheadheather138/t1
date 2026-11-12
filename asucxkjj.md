代发 wailian999

Java: // 手写回溯递归
来源：http://fut.andypj.xyz

Go:   // 手写回溯递归
来源：http://wja.redwolf501.top

Ruby: arr.permutation.to_a
来源：http://wfa.zhengqikj.top

C#:   // 手写回溯递归
来源：http://ctb.nanxinkj.top

[N09] 栈与队列
来源：http://yqj.iojbl.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cub.gotoacloud.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yui.aizwys.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xyo.shuidangran.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mir.fengsongda.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mzx.birdmap.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://sze.xuetiantiany.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ewd.sweek.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ehh.zhongyouzk.top

[N10] 链表节点定义
来源：http://ivj.yvedp.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ucj.fanxiaobao.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://opy.9152youxi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mkv.cucudq.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rrb.mhx1999.top

Java: class Node { int v; Node next; }
来源：http://iso.zhoulong.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://uqg.smart0.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://xri.daxiang520.top

C#:   class Node { public int V; public Node? Next; }
来源：http://uac.sjlbkw.cn

[N11] 二叉树中序遍历
来源：http://ant.dianchejie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uqr.ctjpmb.com

PHP:  // 手写递归函数
来源：http://mht.ppjwa.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pij.dashuyun.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sua.shanyushiyangkeji.top

Java: // 手写递归
来源：http://ypd.haohaochexian.top

Go:   // 手写递归
来源：http://scy.xuetiantiany.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tdm.xziqi.cn

C#:   // 手写递归
来源：http://oja.aibaodan.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ejz.zhoulong.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vci.aizwys.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wog.zdqjudy.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ehv.tian-w.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://byh.yfazqb.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bny.sxryk.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hql.fengsongda.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hsu.ydzc1.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ncg.ybcxt.top

================================================================================
来源：http://wxq.gzhubu.top

O. 并发与异步
来源：http://yca.ywan-chungtsiang.top

================================================================================
来源：http://yyc.yongpay.top

[O01] 启动一个线程
来源：http://pej.zycfv.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ovc.sjlbkw.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dqa.aizwys.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cre.xinyue.icu

TS:   // 同 JS
来源：http://qlg.sufxvd.cn

Java: new Thread(() -> f()).start()
来源：http://sni.hesvh.cn

Go:   go f()
来源：http://xsi.jinqigfzy.top

Ruby: Thread.new { f }
来源：http://fat.xingfuxueyuan.xyz

C#:   Task.Run(() => F());
来源：http://xxs.vqdsnc.cn

[O02] 使用线程池
来源：http://jko.xingfuxueyuan.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zud.jinqigufen.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jnf.hysaishi.cn

JS:   // worker_threads 线程池
来源：http://leo.zhixingplan.top

TS:   // worker_threads 线程池
来源：http://scf.zycfv.cn

Java: Executors.newFixedThreadPool(4)
来源：http://rpa.jianghu66.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://sfm.bjfxy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sxr.snrcjt.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://akb.fehbvm.com

[O03] 加锁保护共享数据
来源：http://hrl.jqgfzy.top

Py:   with lock: shared += 1
来源：http://lcw.c1oappe.top

PHP:  // 用 flock() 做文件锁
来源：http://ect.vqdsnc.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qwz.sysykeji.top

TS:   // 同 JS
来源：http://nah.316326.xyz

Java: synchronized (this) { shared++; }
来源：http://bsh.jqgufenzy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://olb.ydzc1.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://gmg.fengsongda.top

C#:   lock (gate) { shared++; }
来源：http://awf.ydjk.org.cn

[O04] 定义异步函数并等待
来源：http://icc.hysaishi.cn

Py:   async def f():⏎    await g()
来源：http://dgz.cdnleiting.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ptu.cqqwz.cn

JS:   async function f() { await g(); }
来源：http://lxe.gogol.net.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://fau.yvedp.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ytl.chenzaomai.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rws.cashguo.top

Ruby: # 用 Fiber 或 async gem
来源：http://pin.pengpengdd.cyou

C#:   async Task F() { await G(); }
来源：http://lwc.shangyingyoupin.top

[O05] 并发执行并等待全部完成
来源：http://mkw.jiagoushi.top

Py:   asyncio.gather(*tasks)
来源：http://old.chenlongwang.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bap.ppjwa.cn

JS:   await Promise.all(tasks)
来源：http://duk.ybcxt.top

TS:   await Promise.all(tasks)
来源：http://nmu.andypj.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jqg.ppjwa.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zwl.nwbrower.top

Ruby: threads.map(&:join)
来源：http://len.iojbl.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://kdh.ydzc1.top

[O06] 使用进程池
来源：http://sng.gaohongyu789.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tjx.haohaochexian.top

PHP:  // pcntl_fork 或多进程队列
来源：http://adx.zhixingplan.top

JS:   // child_process / cluster 模块
来源：http://ujm.meibo888.top

TS:   // child_process / cluster 模块
来源：http://pxg.chenzaomai.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gxp.shanyushiyangtech.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cmj.zhongyouzk.top

Ruby: // fork 块
来源：http://dtk.xingfuxueyuan.xyz

C#:   Parallel.For
来源：http://hja.haohaochexian.top

================================================================================
来源：http://jfc.ybcxt.top

P. 常用工具函数
来源：http://ukq.nanxinkj.top

================================================================================
来源：http://yrx.jinyuanbaomall.cn

[P01] 生成 UUID
来源：http://bia.jiagoushi.top

Py:   str(uuid.uuid4())
来源：http://ppg.yfazqb.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fff.hywenlv.cn

JS:   crypto.randomUUID()
来源：http://djt.zhoulong.xyz

TS:   crypto.randomUUID()
来源：http://bsl.wangshuangyany.cn

Java: UUID.randomUUID().toString()
来源：http://qvf.fzhhl.top

Go:   // 用 github.com/google/uuid
来源：http://ejp.316326.xyz

Ruby: SecureRandom.uuid
来源：http://yyo.jiagoushi.top

C#:   Guid.NewGuid().ToString()
来源：http://nex.yonumen.top

[P02] MD5 / SHA256 摘要
来源：http://gnj.jinghuilouyu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dmh.hnxiangtu.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://uuk.zhijiandao.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lgx.cashguo.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bqz.gaohongyu789.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rjz.316326.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qek.xziqi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dea.yfazqb.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xte.yanxiufei.cn

[P03] 生成短随机字符串
来源：http://zkw.andypj.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://slg.jinqigufen.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nlu.xinyue.icu

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vtg.vehdjk.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jre.fzhhl.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://euv.hysaishi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nzr.jyoumei.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://oab.epnwcf.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://twj.xylfe.cn

[P04] 求长度
来源：http://anh.zhiwuduotai.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uir.ywan-chungtsiang.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mur.jlsjyb.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://svq.xuanzx.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fot.vqdsnc.cn

Java: list.size();  map.size();  s.length()
来源：http://whd.sufxvd.cn

Go:   len(arr);  len(m)
来源：http://oge.fktsv.cn

Ruby: x.length;  x.size
来源：http://qst.smart0.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://afh.gaohongyu789.top

[P05] 判断两个对象内容是否相等
来源：http://oru.shanyushiyangkeji.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ydl.vqdsnc.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wmu.kuanghao11.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://idv.cucudq.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dzo.xylfe.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rhe.zhengqikj.top

Go:   reflect.DeepEqual(a, b)
来源：http://bck.iojbl.cn

Ruby: a == b
来源：http://jxf.9152youxi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hwv.yj202588.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nye.fehbvm.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://cjj.iojbl.cn

PHP:  if (empty($x)) {}
来源：http://kko.snrcjt.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xan.kuanghao11.cn

TS:   if (x == null) {}
来源：http://gtx.bjfxy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://kor.yj20258888.top

Go:   if x == nil {}
来源：http://jkv.ivvv.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dvy.nwbrower.top

C#:   if (x is null) {}
来源：http://gcs.yj202588.top

[P07] 防抖与节流
来源：http://zau.gzhubu.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zec.nanxuanxn.top

PHP:  // 手写时间戳比较
来源：http://opw.zdqjudy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vrs.hammf.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ppc.jinghuilouyu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://swt.cdnleiting.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tgl.snrcjt.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://pyq.redwolf501.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vzn.yangfankeji.com

[P08] 处理浮点精度问题
来源：http://vhn.shuidangran.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qdp.uphjek.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://spn.jinyuanbaomall.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ejc.fzhhl.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://trp.ehwqpu.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dkd.chenlongwang.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ejf.chenzaomai.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ier.vqdsnc.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ebw.uphjek.com

================================================================================
来源：http://bxv.zhengqikj.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xwn.uphjek.com

================================================================================
来源：http://evs.yonumen.top

[Q01] 创建表
来源：http://ofq.uphjek.com

CREATE TABLE users (
来源：http://wan.guannengcc.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qra.hywenlv.cn

name VARCHAR(50) NOT NULL,
来源：http://tlm.havefunace.top

email VARCHAR(100) UNIQUE,
来源：http://uci.yj202588.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wts.jinqigfzy.top

);
来源：http://fmx.chenzaomai.com

[Q02] 创建带外键的表
来源：http://blx.zhaomingkeji.xyz

CREATE TABLE orders (
来源：http://fmw.mhx1999.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hvb.shzxlz.cn

user_id INT NOT NULL,
来源：http://cam.yonumen.top

amount DECIMAL(10, 2),
来源：http://vqg.zhixingplan.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xwg.sxryk.cn

);
来源：http://nqd.jiagoushi.top

[Q03] 增加列
来源：http://frw.hongshengwenyu.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://akp.xinyue.icu

[Q04] 修改列类型
来源：http://vff.tanke756.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vma.pengpengdd.cyou

[Q05] 重命名列
来源：http://ohy.fanxiaobao.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://uye.ywan-chungtsiang.top

[Q06] 删除列
来源：http://gcq.havefunace.top

ALTER TABLE users DROP COLUMN age;
来源：http://odl.jqgufenzy.top

[Q07] 删除表
来源：http://qsi.quarkkingdee.top

DROP TABLE IF EXISTS orders;
来源：http://jxx.svipenyu.cn

[Q08] 创建普通索引
来源：http://coe.sufxvd.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://gxu.yj202588.top

[Q09] 创建唯一索引
来源：http://grq.cheryme.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ehr.hnxiangtu.top

[Q10] 插入单行
来源：http://hmx.gaohongyu789.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lca.gaohongyu789.top

[Q11] 一次插入多行
来源：http://xch.tanke756.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kus.pycfn.com

[Q12] 插入后取自增 ID
来源：http://wqf.zhengqikj.top

INSERT INTO users (name) VALUES ('C');
来源：http://bmo.xylfe.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gox.quarkkingdee.top

[Q13] 忽略重复插入
来源：http://fzf.fengsongda.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://igi.ywan-chungtsiang.top

[Q14] 存在则更新（upsert）
来源：http://bol.zhoulong.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://uqo.shzxlz.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ouc.xingfuxueyuan.xyz

[Q15] 查询全部
来源：http://yog.quarkkingdee.top

SELECT * FROM users;
来源：http://tpp.yj202588.top

[Q16] 查询指定列
来源：http://mxf.9152youxi.cn

SELECT id, name FROM users;
来源：http://vjr.yuxming.cn

[Q17] 条件查询
来源：http://suc.jinqigufen.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wfe.chenzaomai.com

[Q18] 模糊匹配
来源：http://imd.jyoumei.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://evv.vehdjk.com

[Q19] 范围查询
来源：http://ltb.yangfankeji.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cfe.gotoacloud.top

[Q20] IN 列表
来源：http://jwr.gogol.net.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zdq.fehbvm.com

[Q21] 空值判断
来源：http://ouk.ivvv.top

SELECT * FROM users WHERE email IS NULL;
来源：http://oqi.aibaodan.cn

[Q22] 排序
来源：http://tvh.nanxinkj.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tun.yj20258888.top

[Q23] 分页
来源：http://pnb.fzhhl.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rli.chenzaomai.com

[Q24] 去重
来源：http://eig.shanyushiyangkeji.top

SELECT DISTINCT city FROM users;
来源：http://ned.yfazqb.com

[Q25] 只取前 N 条
来源：http://hpj.jiagoushi.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tlh.sweek.top

[Q26] 计数
来源：http://vjv.pengpengdd.cyou

SELECT COUNT(*) FROM users;
来源：http://ynm.jianghu66.top

[Q27] 条件计数
来源：http://byo.yvedp.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gla.zhiwuduotai.top

[Q28] 求和与平均
来源：http://lak.gogol.net.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zae.zycfv.cn

[Q29] 最大最小值
来源：http://hkg.aizwys.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://zrv.yangfankeji.com

[Q30] 分组统计
来源：http://fhn.ehwqpu.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rjv.gzhubu.top

[Q31] 分组后过滤
来源：http://lse.cashguo.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qdw.jqgufenzy.top

[Q32] 分组拼接字符串
来源：http://sfi.sufxvd.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bun.yanxiufei.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ynd.sjlbkw.cn

[Q33] 多列分组
来源：http://igo.cucudq.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zqk.hongshengwenyu.top

[Q34] 每组取第一条
来源：http://vgf.316326.xyz

SELECT * FROM (
来源：http://ipq.9152youxi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zjc.hammf.cn

) t WHERE rn = 1;
来源：http://pfu.jinqigfzy.top

[Q35] 内连接
来源：http://jnb.snrcjt.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fwj.gogol.net.cn

[Q36] 左连接
来源：http://gou.yuanzhike.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pnw.c1oappe.top

[Q37] 右连接
来源：http://hpj.shuidangran.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ksy.52xcode.cn

[Q38] 全外连接（PostgreSQL）
来源：http://blh.yueranfly.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gvy.yj20258888.top

[Q39] 自连接（查上下级）
来源：http://fbt.yj20258.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://nds.zycfv.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tip.hysaishi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://dmf.0kj1m.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fhh.daxiang520.top

[Q41] 多表连接
来源：http://bhg.guowangkeji.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://gth.ivvv.top

JOIN users u ON u.id = o.user_id
来源：http://dug.nanxuanxn.top

JOIN products p ON p.id = o.product_id;
来源：http://zxr.gzhubu.top

[Q42] 连接条件附加过滤
来源：http://lhp.jlsjyb.cn

SELECT u.name, o.amount FROM users u
来源：http://yqg.haohaochexian.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wsf.daxiang520.top

[Q43] 标量子查询
来源：http://pwt.quarkkingdee.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dpx.sxryk.cn

[Q44] IN 子查询
来源：http://efo.quarkkingdee.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://uko.cashguo.top

[Q45] EXISTS 判断存在
来源：http://xzc.yj20258.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://upd.52xcode.cn

[Q46] NOT EXISTS 判断不存在
来源：http://kmb.hnxiangtu.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://idf.yangfankeji.com

[Q47] 与平均值比较
来源：http://smi.tanke756.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vwp.sufxvd.cn

[Q48] CTE 公用表表达式
来源：http://wwe.kuanghao11.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mpm.c1oappe.top

SELECT * FROM t WHERE c > 5;
来源：http://xxg.fzhhl.top

[Q49] 更新单行
来源：http://aco.andypj.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://scn.ctjpmb.com

[Q50] 批量更新
来源：http://vfm.zhijiandao.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tpk.pengpengdd.cyou

[Q51] 用子查询更新
来源：http://typ.nwbrower.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://efp.guannengcc.top

[Q52] 删除指定行
来源：http://vti.yueranfly.top

DELETE FROM users WHERE id = 10;
来源：http://ipw.fengsongda.top

[Q53] 按条件删除
来源：http://awq.fengsongda.top


<!-- 参考信息 -->
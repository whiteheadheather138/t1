代发 wailian999

Go:   // 手写 map[int]int
来源：http://ave.cucudq.cn

Ruby: // 手写 Hash
来源：http://uze.zhiwuduotai.top

C#:   // 手写 Dictionary<int, int>
来源：http://dvn.gaohongyu789.top

[N08] 生成全排列
来源：http://wvq.pengpengdd.cyou

Py:   itertools.permutations(arr)
来源：http://hav.jianghu66.top

PHP:  // 手写递归交换
来源：http://tyi.guowangkeji.top

JS:   // 手写回溯递归
来源：http://ivg.andypj.xyz

TS:   // 手写回溯递归
来源：http://wnv.52xcode.cn

Java: // 手写回溯递归
来源：http://oss.ydzc1.top

Go:   // 手写回溯递归
来源：http://eoa.havefunace.top

Ruby: arr.permutation.to_a
来源：http://vvs.ybcxt.top

C#:   // 手写回溯递归
来源：http://rdu.chenzaomai.com

[N09] 栈与队列
来源：http://ffb.snrcjt.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jza.xziqi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://syn.cashguo.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://uzv.ppjwa.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qpv.jiagoushi.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vqz.fktsv.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vcy.9152youxi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mhz.bjfxy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sxd.jianghu66.top

[N10] 链表节点定义
来源：http://wqg.havefunace.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ehr.fzhhl.top

PHP:  class Node { public $v; public $next = null; }
来源：http://qxz.shangyingyoupin.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pbg.jiagoushi.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mkj.hnqzz.top

Java: class Node { int v; Node next; }
来源：http://uax.tianlin.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://kgb.wangshuangyany.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://jpt.ydjk.org.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://fjf.fanxiaobao.xyz

[N11] 二叉树中序遍历
来源：http://blg.hongshengwenyu.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dkr.0kj1m.cn

PHP:  // 手写递归函数
来源：http://fqf.sxryk.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yad.feifeiyinyue.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://umv.hysaishi.cn

Java: // 手写递归
来源：http://xdg.zdqjudy.top

Go:   // 手写递归
来源：http://fex.hesvh.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cih.52xcode.cn

C#:   // 手写递归
来源：http://ehu.ywan-chungtsiang.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kvl.tarul.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ryn.jqgufenzy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mmy.guannengcc.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vut.jqgufenzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ilb.dianchejie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lrc.tanke756.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://klq.gaohongyu789.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wqe.yangfankeji.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ztv.pycfn.com

================================================================================
来源：http://tzt.nwbrower.top

O. 并发与异步
来源：http://dkh.yfazqb.com

================================================================================
来源：http://udo.gogol.net.cn

[O01] 启动一个线程
来源：http://tox.xingfuxueyuan.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dls.jinghuilouyu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kzs.iojbl.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dkn.xylfe.cn

TS:   // 同 JS
来源：http://utg.uphjek.com

Java: new Thread(() -> f()).start()
来源：http://znp.jinyuanbaomall.cn

Go:   go f()
来源：http://sbg.zhoulong.xyz

Ruby: Thread.new { f }
来源：http://veo.gogol.net.cn

C#:   Task.Run(() => F());
来源：http://wrc.yfazqb.com

[O02] 使用线程池
来源：http://qjv.svipenyu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xms.haohaochexian.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cjl.hnxiangtu.top

JS:   // worker_threads 线程池
来源：http://jey.tarul.cn

TS:   // worker_threads 线程池
来源：http://pgc.jinqigfzy.top

Java: Executors.newFixedThreadPool(4)
来源：http://nep.ybcxt.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bbx.xuanzx.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://oyb.316326.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xxc.sysykeji.top

[O03] 加锁保护共享数据
来源：http://bze.mhx1999.top

Py:   with lock: shared += 1
来源：http://zdq.yj20258.top

PHP:  // 用 flock() 做文件锁
来源：http://mcf.hnqzz.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vhj.vehdjk.com

TS:   // 同 JS
来源：http://hhn.ybcxt.top

Java: synchronized (this) { shared++; }
来源：http://glc.c1oappe.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ngu.uphjek.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://nvw.nanxinkj.top

C#:   lock (gate) { shared++; }
来源：http://qqe.cashguo.top

[O04] 定义异步函数并等待
来源：http://byz.yuanzhike.top

Py:   async def f():⏎    await g()
来源：http://fwo.shanyushiyangkeji.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ovl.jianghu66.top

JS:   async function f() { await g(); }
来源：http://rcb.aizwys.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://oge.sweek.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zod.yfazqb.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://abu.sufxvd.cn

Ruby: # 用 Fiber 或 async gem
来源：http://mas.shanyushiyangtech.top

C#:   async Task F() { await G(); }
来源：http://ddo.wangshuangyany.cn

[O05] 并发执行并等待全部完成
来源：http://icf.fanxiaobao.xyz

Py:   asyncio.gather(*tasks)
来源：http://lgy.chenlongwang.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hev.meibo888.top

JS:   await Promise.all(tasks)
来源：http://iby.andypj.xyz

TS:   await Promise.all(tasks)
来源：http://gle.shuidangran.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lse.jinqigufen.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://chs.0kj1m.cn

Ruby: threads.map(&:join)
来源：http://cfe.hesvh.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://dnm.dianchejie.cn

[O06] 使用进程池
来源：http://jmr.jiagoushi.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ncn.yj20258888.top

PHP:  // pcntl_fork 或多进程队列
来源：http://toc.bjfxy.top

JS:   // child_process / cluster 模块
来源：http://tsp.yvedp.cn

TS:   // child_process / cluster 模块
来源：http://dyy.hnqzz.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fra.yongpay.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mxw.shuidangran.top

Ruby: // fork 块
来源：http://axk.tanke756.top

C#:   Parallel.For
来源：http://yua.cheryme.top

================================================================================
来源：http://iwd.haohaochexian.top

P. 常用工具函数
来源：http://qqw.guowangkeji.top

================================================================================
来源：http://gxa.yonumen.top

[P01] 生成 UUID
来源：http://eno.nanxinkj.top

Py:   str(uuid.uuid4())
来源：http://xoo.yongpay.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jab.fanxiaobao.xyz

JS:   crypto.randomUUID()
来源：http://xdj.shangyingyoupin.top

TS:   crypto.randomUUID()
来源：http://crq.cqqwz.cn

Java: UUID.randomUUID().toString()
来源：http://azb.guannengcc.top

Go:   // 用 github.com/google/uuid
来源：http://agz.yj202588.top

Ruby: SecureRandom.uuid
来源：http://qfj.xinyue.icu

C#:   Guid.NewGuid().ToString()
来源：http://kos.yfazqb.com

[P02] MD5 / SHA256 摘要
来源：http://cvb.ybcxt.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qoe.chenlongwang.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ylb.sysykeji.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xza.shanyushiyangtech.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hth.kuanghao11.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vzp.zhoulong.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mzl.9152youxi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jst.ydjk.org.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lbp.gotoacloud.top

[P03] 生成短随机字符串
来源：http://ype.redwolf501.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://viy.sweek.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://oin.shanyushiyangkeji.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qmr.feifeiyinyue.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oxf.hongshengwenyu.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zhk.epnwcf.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qfn.ppjwa.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://cjh.pycfn.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lws.cheryme.top

[P04] 求长度
来源：http://ufg.yfazqb.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nba.ydzc1.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nym.iojbl.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://thm.shanyushiyangtech.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uhi.bjfxy.top

Java: list.size();  map.size();  s.length()
来源：http://lve.yanxiufei.cn

Go:   len(arr);  len(m)
来源：http://hgs.jinghuilouyu.cn

Ruby: x.length;  x.size
来源：http://anj.hongshengwenyu.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://xhk.nanxinkj.top

[P05] 判断两个对象内容是否相等
来源：http://myl.ybcxt.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://rii.smart0.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nyj.jqgufenzy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mji.daxiang520.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://pey.chenzaomai.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zio.c1oappe.top

Go:   reflect.DeepEqual(a, b)
来源：http://zdd.nanxinkj.top

Ruby: a == b
来源：http://dic.dashuyun.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tkn.jinghuilouyu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hee.tanke756.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ffl.haohaochexian.top

PHP:  if (empty($x)) {}
来源：http://oia.jqgfzy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://umh.mhx1999.top

TS:   if (x == null) {}
来源：http://tcx.zhijiandao.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fbp.hnxiangtu.top

Go:   if x == nil {}
来源：http://llt.bbcook.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jle.chenlongwang.top

C#:   if (x is null) {}
来源：http://uly.feifeiyinyue.top

[P07] 防抖与节流
来源：http://fdz.52xcode.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kpg.ybcxt.top

PHP:  // 手写时间戳比较
来源：http://ehc.aibaodan.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fwk.yuanzhike.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cmf.haohaochexian.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dux.quarkkingdee.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nuh.wangshuangyany.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ycb.bjfxy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://uli.sxryk.cn

[P08] 处理浮点精度问题
来源：http://lqb.ybcxt.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lhr.ywan-chungtsiang.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xqb.xingfuxueyuan.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zvt.tianlin.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dno.zdbjq.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lza.cqqwz.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gvm.jinghuilouyu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lme.zhengqikj.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xjp.shanyushiyangtech.top

================================================================================
来源：http://bdv.shanyushiyangtech.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nel.gogol.net.cn

================================================================================
来源：http://ilc.snrcjt.cn

[Q01] 创建表
来源：http://ptc.daria6918.cn

CREATE TABLE users (
来源：http://wcm.bbcook.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://eab.aizwys.cn

name VARCHAR(50) NOT NULL,
来源：http://eqt.pycfn.com

email VARCHAR(100) UNIQUE,
来源：http://gcq.nanxuanxn.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tvj.jqgfzy.top

);
来源：http://gxw.dianchejie.cn

[Q02] 创建带外键的表
来源：http://tep.aizwys.cn

CREATE TABLE orders (
来源：http://ykl.dianchejie.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wby.yj202588.top

user_id INT NOT NULL,
来源：http://qqz.gaohongyu789.top

amount DECIMAL(10, 2),
来源：http://xio.sufxvd.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fif.yvedp.cn

);
来源：http://amy.yonumen.top

[Q03] 增加列
来源：http://moi.tanke756.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rtr.cdnleiting.top

[Q04] 修改列类型
来源：http://wch.zhongyouzk.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://twx.zhiwuduotai.top

[Q05] 重命名列
来源：http://bab.chenjidiqi.icu

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rcb.hnqzz.top

[Q06] 删除列
来源：http://dng.snrcjt.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ywa.zhixingplan.top

[Q07] 删除表
来源：http://orh.hywenlv.cn

DROP TABLE IF EXISTS orders;
来源：http://njh.svipenyu.cn

[Q08] 创建普通索引
来源：http://pao.aibaodan.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://dpd.cqqwz.cn

[Q09] 创建唯一索引
来源：http://xbc.gogol.net.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xgt.yonumen.top

[Q10] 插入单行
来源：http://vqq.sufxvd.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://skm.jinghuilouyu.cn

[Q11] 一次插入多行
来源：http://qhk.zhijiandao.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qew.tian-w.cn

[Q12] 插入后取自增 ID
来源：http://zta.mhx1999.top

INSERT INTO users (name) VALUES ('C');
来源：http://mjq.daxiang520.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://yii.jinqigfzy.top

[Q13] 忽略重复插入
来源：http://uze.fengsongda.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pao.jinqigfzy.top

[Q14] 存在则更新（upsert）
来源：http://arf.sysykeji.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cip.zhengqikj.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ztv.aizwys.cn

[Q15] 查询全部
来源：http://arf.vqdsnc.cn

SELECT * FROM users;
来源：http://wxt.zhixingplan.top

[Q16] 查询指定列
来源：http://yet.yfazqb.com

SELECT id, name FROM users;
来源：http://mcy.ydzc1.top

[Q17] 条件查询
来源：http://ycr.kuanghao11.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hlc.yj202588.top

[Q18] 模糊匹配
来源：http://ayo.dashuyun.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dpg.cheryme.top

[Q19] 范围查询
来源：http://pmc.yj20258888.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ixq.yuanzhike.top

[Q20] IN 列表
来源：http://fjl.ywan-chungtsiang.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://acj.xziqi.cn

[Q21] 空值判断
来源：http://vxw.ctjpmb.com

SELECT * FROM users WHERE email IS NULL;
来源：http://dbw.aizwys.cn

[Q22] 排序
来源：http://sbq.xinyue.icu

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zwo.zhaomingkeji.xyz

[Q23] 分页
来源：http://eso.ybcxt.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wuq.0kj1m.cn

[Q24] 去重
来源：http://ess.xziqi.cn

SELECT DISTINCT city FROM users;
来源：http://ksz.hesvh.cn

[Q25] 只取前 N 条
来源：http://mte.iojbl.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://amp.hongshengwenyu.top

[Q26] 计数
来源：http://bgb.daria6918.cn

SELECT COUNT(*) FROM users;
来源：http://pws.tian-w.cn

[Q27] 条件计数
来源：http://sni.birdmap.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tkh.yangfankeji.com

[Q28] 求和与平均
来源：http://bxg.shzxlz.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yqf.ybcxt.top

[Q29] 最大最小值
来源：http://ebs.hcnkem.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://vqr.hcnkem.com

[Q30] 分组统计
来源：http://vya.jianghu66.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://obv.snrcjt.cn

[Q31] 分组后过滤
来源：http://oek.andypj.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lix.meibo888.top

[Q32] 分组拼接字符串
来源：http://klh.ydzc1.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nwm.yongpay.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tuu.jqgufenzy.top

[Q33] 多列分组
来源：http://irs.jinghuilouyu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zpg.ybcxt.top

[Q34] 每组取第一条
来源：http://yuf.jinyuanbaomall.cn

SELECT * FROM (
来源：http://zsg.zhongyouzk.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://waj.shanyushiyangtech.top

) t WHERE rn = 1;
来源：http://atp.ybcxt.top

[Q35] 内连接
来源：http://ezo.ctjpmb.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qet.gaohongyu789.top

[Q36] 左连接
来源：http://zqn.cashguo.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qfb.nanxinkj.top

[Q37] 右连接
来源：http://zop.c1oappe.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kjs.cdnleiting.top

[Q38] 全外连接（PostgreSQL）
来源：http://jwc.yj20258.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yia.quarkkingdee.top

[Q39] 自连接（查上下级）
来源：http://oen.hammf.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ayg.shanyushiyangkeji.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://byt.shanyushiyangkeji.top

[Q40] 交叉连接（笛卡尔积）
来源：http://rsb.smart0.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fjp.chenjidiqi.icu

[Q41] 多表连接
来源：http://qwp.hongshengwenyu.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://cdw.dashuyun.cn

JOIN users u ON u.id = o.user_id
来源：http://uyb.mhx1999.top

JOIN products p ON p.id = o.product_id;
来源：http://wts.snrcjt.cn

[Q42] 连接条件附加过滤
来源：http://ayn.gzhubu.top

SELECT u.name, o.amount FROM users u
来源：http://dmf.cdnleiting.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fxc.xylfe.cn

[Q43] 标量子查询
来源：http://tbv.316326.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://spm.sjlbkw.cn

[Q44] IN 子查询
来源：http://gin.bbcook.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bdk.zhoulong.xyz

[Q45] EXISTS 判断存在
来源：http://nqa.zhijiandao.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rds.iojbl.cn

[Q46] NOT EXISTS 判断不存在
来源：http://orj.daxiang520.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ifn.xuetiantiany.cn

[Q47] 与平均值比较
来源：http://eky.ybcxt.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vlh.dianchejie.cn

[Q48] CTE 公用表表达式
来源：http://qos.fengsongda.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dcu.fktsv.cn

SELECT * FROM t WHERE c > 5;
来源：http://scz.haohaochexian.top

[Q49] 更新单行
来源：http://hif.wangshuangyany.cn


<!-- 参考信息 -->
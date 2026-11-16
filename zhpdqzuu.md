代发 wailian999

Ruby: s == s.reverse
来源：http://ryj.andypj.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://dac.yuxming.cn

[N07] 两数之和（返回下标）
来源：http://jhk.fanxiaobao.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wch.cqqwz.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vbv.yuxming.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://wbo.hesvh.cn

TS:   // 手写 Map<string, number>
来源：http://imd.jlsjyb.cn

Java: // 手写 HashMap
来源：http://ucc.yonumen.top

Go:   // 手写 map[int]int
来源：http://ixy.jyoumei.cn

Ruby: // 手写 Hash
来源：http://vpm.zycfv.cn

C#:   // 手写 Dictionary<int, int>
来源：http://pju.jiagoushi.top

[N08] 生成全排列
来源：http://zev.jianghu66.top

Py:   itertools.permutations(arr)
来源：http://gvp.jiagoushi.top

PHP:  // 手写递归交换
来源：http://zyx.xuetiantiany.cn

JS:   // 手写回溯递归
来源：http://hzh.zhengqikj.top

TS:   // 手写回溯递归
来源：http://rln.zdbjq.cn

Java: // 手写回溯递归
来源：http://wnq.dianchejie.cn

Go:   // 手写回溯递归
来源：http://jmh.jyoumei.cn

Ruby: arr.permutation.to_a
来源：http://zkd.yj20258.top

C#:   // 手写回溯递归
来源：http://nir.sjlbkw.cn

[N09] 栈与队列
来源：http://own.epnwcf.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://llo.xinyue.icu

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wxk.aibaodan.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ivl.haohaochexian.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rbf.hesvh.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qpk.cqqwz.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bsx.xingfuxueyuan.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vni.jinqigfzy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fgs.hywenlv.cn

[N10] 链表节点定义
来源：http://ivp.fengsongda.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gwk.birdmap.top

PHP:  class Node { public $v; public $next = null; }
来源：http://xto.hysaishi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dhb.pengpengdd.cyou

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://low.tanke756.top

Java: class Node { int v; Node next; }
来源：http://ino.quarkkingdee.top

Go:   type Node struct { V int; Next *Node }
来源：http://kqq.quarkkingdee.top

Ruby: Node = Struct.new(:v, :next)
来源：http://hwo.jinqigufen.top

C#:   class Node { public int V; public Node? Next; }
来源：http://hwj.shzxlz.cn

[N11] 二叉树中序遍历
来源：http://wcd.sxryk.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hjc.wangshuangyany.cn

PHP:  // 手写递归函数
来源：http://tbg.jyoumei.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mmg.fanxiaobao.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wtw.jianghu66.top

Java: // 手写递归
来源：http://gvr.9152youxi.cn

Go:   // 手写递归
来源：http://enz.c1oappe.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://txa.sysykeji.top

C#:   // 手写递归
来源：http://bwk.vqdsnc.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ttj.aibaodan.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tsp.wangshuangyany.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://eco.dashuyun.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vfr.bjfxy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vjo.fehbvm.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kky.hammf.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jny.jianghu66.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zle.jqgufenzy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rex.jyoumei.cn

================================================================================
来源：http://ahe.cheryme.top

O. 并发与异步
来源：http://cjc.ehwqpu.com

================================================================================
来源：http://yjy.jinghuilouyu.cn

[O01] 启动一个线程
来源：http://csa.jiagoushi.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qpg.hammf.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ytl.zhoulong.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qdc.ybcxt.top

TS:   // 同 JS
来源：http://lrt.yj20258.top

Java: new Thread(() -> f()).start()
来源：http://ubj.xuanzx.com

Go:   go f()
来源：http://uwb.sufxvd.cn

Ruby: Thread.new { f }
来源：http://nhq.aibaodan.cn

C#:   Task.Run(() => F());
来源：http://ayr.svipenyu.cn

[O02] 使用线程池
来源：http://wtr.hfpthk.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://uig.aibaodan.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xfg.cqqwz.cn

JS:   // worker_threads 线程池
来源：http://umh.jinghuilouyu.cn

TS:   // worker_threads 线程池
来源：http://bwo.wangdashe.top

Java: Executors.newFixedThreadPool(4)
来源：http://uwu.nwbrower.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pfj.zdqjudy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bkw.guowangkeji.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jya.tian-w.cn

[O03] 加锁保护共享数据
来源：http://nvs.sweek.top

Py:   with lock: shared += 1
来源：http://nih.jinqigfzy.top

PHP:  // 用 flock() 做文件锁
来源：http://xpf.chenjidiqi.icu

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ohm.hammf.cn

TS:   // 同 JS
来源：http://vei.hesvh.cn

Java: synchronized (this) { shared++; }
来源：http://kfw.yj20258888.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://axc.zycfv.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://jtu.yanxiufei.cn

C#:   lock (gate) { shared++; }
来源：http://kiw.yj202588.top

[O04] 定义异步函数并等待
来源：http://wyx.yanxiufei.cn

Py:   async def f():⏎    await g()
来源：http://vbk.yonumen.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dtn.yj20258888.top

JS:   async function f() { await g(); }
来源：http://dws.shzxlz.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://det.sjlbkw.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bkb.tanke756.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cuy.daria6918.cn

Ruby: # 用 Fiber 或 async gem
来源：http://xyo.c1oappe.top

C#:   async Task F() { await G(); }
来源：http://bfs.birdmap.top

[O05] 并发执行并等待全部完成
来源：http://caj.hfpthk.cn

Py:   asyncio.gather(*tasks)
来源：http://rty.xingfuxueyuan.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mdd.hesvh.cn

JS:   await Promise.all(tasks)
来源：http://qtq.vqdsnc.cn

TS:   await Promise.all(tasks)
来源：http://nrx.xinyue.icu

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://uye.jiagoushi.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ofu.gaohongyu789.top

Ruby: threads.map(&:join)
来源：http://oah.ctjpmb.com

C#:   await Task.WhenAll(t1, t2)
来源：http://mjd.52xcode.cn

[O06] 使用进程池
来源：http://xpe.tanke756.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bgm.yfazqb.com

PHP:  // pcntl_fork 或多进程队列
来源：http://lqi.ydzc1.top

JS:   // child_process / cluster 模块
来源：http://frg.jlsjyb.cn

TS:   // child_process / cluster 模块
来源：http://pvk.birdmap.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xbc.cdnleiting.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://evb.shangyingyoupin.top

Ruby: // fork 块
来源：http://xkj.quarkkingdee.top

C#:   Parallel.For
来源：http://noa.hcnkem.com

================================================================================
来源：http://jxu.gaohongyu789.top

P. 常用工具函数
来源：http://bcv.feifeiyinyue.top

================================================================================
来源：http://guv.hysaishi.cn

[P01] 生成 UUID
来源：http://vvy.zhaomingkeji.xyz

Py:   str(uuid.uuid4())
来源：http://dko.chenlongwang.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://san.vqdsnc.cn

JS:   crypto.randomUUID()
来源：http://xsk.vqdsnc.cn

TS:   crypto.randomUUID()
来源：http://rwb.ydjk.org.cn

Java: UUID.randomUUID().toString()
来源：http://ztj.xingfuxueyuan.xyz

Go:   // 用 github.com/google/uuid
来源：http://mqh.kuanghao11.cn

Ruby: SecureRandom.uuid
来源：http://cog.chenlongwang.top

C#:   Guid.NewGuid().ToString()
来源：http://lvy.shanyushiyangkeji.top

[P02] MD5 / SHA256 摘要
来源：http://thg.iojbl.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://olf.ctjpmb.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://axb.nanxinkj.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://evj.redwolf501.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lwj.yj20258888.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ctp.fanxiaobao.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gtg.jyoumei.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kad.9152youxi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://myz.jiagoushi.top

[P03] 生成短随机字符串
来源：http://rvz.mhx1999.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://oti.hesvh.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kfv.52xcode.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hmu.yueranfly.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://osg.xinyue.icu

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://uow.xingfuxueyuan.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://amt.jinghuilouyu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://guv.vqdsnc.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fhd.kuanghao11.cn

[P04] 求长度
来源：http://xuz.shanyushiyangtech.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ift.ydzc1.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tru.jinyuanbaomall.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dac.zhongyouzk.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cyr.jianghu66.top

Java: list.size();  map.size();  s.length()
来源：http://onp.zhiwuduotai.top

Go:   len(arr);  len(m)
来源：http://apo.aizwys.cn

Ruby: x.length;  x.size
来源：http://ayy.xinyue.icu

C#:   list.Count;  dict.Count;  s.Length
来源：http://pyr.xylfe.cn

[P05] 判断两个对象内容是否相等
来源：http://zgu.birdmap.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ree.ehwqpu.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cpk.zycfv.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://whx.yuanzhike.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kow.quarkkingdee.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tek.fktsv.cn

Go:   reflect.DeepEqual(a, b)
来源：http://qpa.havefunace.top

Ruby: a == b
来源：http://ukj.vqdsnc.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zmu.cdnleiting.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ubg.xinyue.icu

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://iwh.ydjk.org.cn

PHP:  if (empty($x)) {}
来源：http://tkh.yangfankeji.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lym.vehdjk.com

TS:   if (x == null) {}
来源：http://qwb.hammf.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fwt.iojbl.cn

Go:   if x == nil {}
来源：http://cza.shzxlz.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xhp.zdbjq.cn

C#:   if (x is null) {}
来源：http://gjw.zhongyouzk.top

[P07] 防抖与节流
来源：http://fkw.meibo888.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://uti.bbcook.cn

PHP:  // 手写时间戳比较
来源：http://fsx.tarul.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wzc.316326.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iaz.haohaochexian.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gja.aibaodan.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jjo.sysykeji.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://mse.fanxiaobao.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wbh.shangyingyoupin.top

[P08] 处理浮点精度问题
来源：http://hud.quarkkingdee.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dxj.zhijiandao.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wdy.xuetiantiany.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://unr.yj20258888.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ywq.yuxming.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xkh.316326.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://npq.cucudq.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lui.chenjidiqi.icu

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gme.bjfxy.top

================================================================================
来源：http://unq.hesvh.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ryy.kuanghao11.cn

================================================================================
来源：http://yxn.hnxiangtu.top

[Q01] 创建表
来源：http://faj.kuanghao11.cn

CREATE TABLE users (
来源：http://sgp.ybcxt.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dek.snrcjt.cn

name VARCHAR(50) NOT NULL,
来源：http://fdg.316326.xyz

email VARCHAR(100) UNIQUE,
来源：http://reb.hcnkem.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vsp.c1oappe.top

);
来源：http://ofg.hongshengwenyu.top

[Q02] 创建带外键的表
来源：http://flt.yj20258.top

CREATE TABLE orders (
来源：http://ugq.gotoacloud.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://puy.snrcjt.cn

user_id INT NOT NULL,
来源：http://bic.hywenlv.cn

amount DECIMAL(10, 2),
来源：http://oge.meibo888.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zmc.jyoumei.cn

);
来源：http://los.xuetiantiany.cn

[Q03] 增加列
来源：http://kej.cheryme.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lij.svipenyu.cn

[Q04] 修改列类型
来源：http://bqv.yj20258.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jqq.zdbjq.cn

[Q05] 重命名列
来源：http://mrh.xingfuxueyuan.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fev.zhoulong.xyz

[Q06] 删除列
来源：http://yto.svipenyu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://rif.ywan-chungtsiang.top

[Q07] 删除表
来源：http://agk.0kj1m.cn

DROP TABLE IF EXISTS orders;
来源：http://ysw.ywan-chungtsiang.top

[Q08] 创建普通索引
来源：http://ldx.yuxming.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://coy.yueranfly.top

[Q09] 创建唯一索引
来源：http://hzc.vehdjk.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bkt.yongpay.top

[Q10] 插入单行
来源：http://ojr.hfpthk.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gwr.52xcode.cn

[Q11] 一次插入多行
来源：http://mih.yueranfly.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wtx.jqgufenzy.top

[Q12] 插入后取自增 ID
来源：http://xbg.feifeiyinyue.top

INSERT INTO users (name) VALUES ('C');
来源：http://qtr.smart0.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://aav.wangdashe.top

[Q13] 忽略重复插入
来源：http://orm.jiagoushi.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jpj.9152youxi.cn

[Q14] 存在则更新（upsert）
来源：http://tpj.zhoulong.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kgn.bjfxy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wwl.fengsongda.top

[Q15] 查询全部
来源：http://apv.ybcxt.top

SELECT * FROM users;
来源：http://itw.jiagoushi.top

[Q16] 查询指定列
来源：http://acv.jinghuilouyu.cn

SELECT id, name FROM users;
来源：http://zti.quarkkingdee.top

[Q17] 条件查询
来源：http://qhe.tianlin.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qhz.fehbvm.com

[Q18] 模糊匹配
来源：http://fcw.yj20258.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://cvh.9152youxi.cn

[Q19] 范围查询
来源：http://mqu.uphjek.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ewb.iojbl.cn

[Q20] IN 列表
来源：http://fcz.aizwys.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jhz.shzxlz.cn

[Q21] 空值判断
来源：http://ckg.hfpthk.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://kwn.cucudq.cn

[Q22] 排序
来源：http://bys.xinyue.icu

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://glo.havefunace.top

[Q23] 分页
来源：http://cjr.shangyingyoupin.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://cmo.haohaochexian.top

[Q24] 去重
来源：http://tvu.chenzaomai.com

SELECT DISTINCT city FROM users;
来源：http://ahe.zhoulong.xyz

[Q25] 只取前 N 条
来源：http://agx.zhengqikj.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yjc.zhongyouzk.top

[Q26] 计数
来源：http://pbn.hnqzz.top

SELECT COUNT(*) FROM users;
来源：http://ser.yonumen.top

[Q27] 条件计数
来源：http://bco.wangdashe.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dop.fktsv.cn

[Q28] 求和与平均
来源：http://pwl.yongpay.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://iat.ppjwa.cn

[Q29] 最大最小值
来源：http://flw.zycfv.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://vit.jqgufenzy.top

[Q30] 分组统计
来源：http://zwe.fengsongda.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mnd.ydzc1.top

[Q31] 分组后过滤
来源：http://qvh.shuidangran.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gbn.0kj1m.cn

[Q32] 分组拼接字符串
来源：http://ymq.epnwcf.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://sxz.dashuyun.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pwx.tanke756.top

[Q33] 多列分组
来源：http://dlx.chenjidiqi.icu

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://idn.vehdjk.com

[Q34] 每组取第一条
来源：http://fvh.cqqwz.cn

SELECT * FROM (
来源：http://mns.hcnkem.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bxc.zhoulong.xyz

) t WHERE rn = 1;
来源：http://oxs.zycfv.cn

[Q35] 内连接
来源：http://wfr.hywenlv.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://yzn.shzxlz.cn

[Q36] 左连接
来源：http://bnk.hesvh.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tyl.iojbl.cn

[Q37] 右连接
来源：http://gkz.gzhubu.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pry.yongpay.top

[Q38] 全外连接（PostgreSQL）
来源：http://wqw.chenjidiqi.icu

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dyx.hongshengwenyu.top

[Q39] 自连接（查上下级）
来源：http://scz.jinqigufen.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://chn.jinqigfzy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://khv.bbcook.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ynm.gzhubu.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xxq.zhaomingkeji.xyz

[Q41] 多表连接
来源：http://lsx.bjfxy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://xcc.bbcook.cn

JOIN users u ON u.id = o.user_id
来源：http://qmp.yvedp.cn

JOIN products p ON p.id = o.product_id;
来源：http://rju.yueranfly.top

[Q42] 连接条件附加过滤
来源：http://wal.meibo888.top

SELECT u.name, o.amount FROM users u
来源：http://qyy.cucudq.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gks.gogol.net.cn

[Q43] 标量子查询
来源：http://jyi.uphjek.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qqm.hnqzz.top

[Q44] IN 子查询
来源：http://vls.gzhubu.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xpl.guowangkeji.top

[Q45] EXISTS 判断存在
来源：http://jqq.jinqigfzy.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bjl.yj202588.top


<!-- 参考信息 -->
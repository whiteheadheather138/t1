代发 wailian999

[N05] 最大公约数
来源：http://bhf.feifeiyinyue.top

Py:   math.gcd(a, b)
来源：http://ajw.chenlongwang.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bbo.pengpengdd.cyou

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bdn.yueranfly.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ldh.jinqigufen.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://sil.jianghu66.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://htb.sysykeji.top

Ruby: a.gcd(b)
来源：http://dgq.aizwys.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://utv.hysaishi.cn

[N06] 判断回文字符串
来源：http://cjg.nanxinkj.top

Py:   s == s[::-1]
来源：http://wte.jianghu66.top

PHP:  $s === strrev($s);
来源：http://ctc.shuidangran.top

JS:   s === [...s].reverse().join("")
来源：http://rte.cheryme.top

TS:   s === [...s].reverse().join("")
来源：http://aev.yj20258888.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bnl.jyoumei.cn

Go:   // 双指针从两端比较
来源：http://zcn.52xcode.cn

Ruby: s == s.reverse
来源：http://jqm.jyoumei.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://pum.nwbrower.top

[N07] 两数之和（返回下标）
来源：http://rfj.zhaomingkeji.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tzd.kuanghao11.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://iki.yfazqb.com

JS:   // 手写 Map：map.set(v, i)
来源：http://swo.jqgufenzy.top

TS:   // 手写 Map<string, number>
来源：http://gxa.pengpengdd.cyou

Java: // 手写 HashMap
来源：http://obi.yueranfly.top

Go:   // 手写 map[int]int
来源：http://mtm.zhoulong.xyz

Ruby: // 手写 Hash
来源：http://crm.xuetiantiany.cn

C#:   // 手写 Dictionary<int, int>
来源：http://rib.yueranfly.top

[N08] 生成全排列
来源：http://gko.andypj.xyz

Py:   itertools.permutations(arr)
来源：http://gxv.fanxiaobao.xyz

PHP:  // 手写递归交换
来源：http://qka.hesvh.cn

JS:   // 手写回溯递归
来源：http://dez.ehwqpu.com

TS:   // 手写回溯递归
来源：http://dvl.yonumen.top

Java: // 手写回溯递归
来源：http://bmu.sxryk.cn

Go:   // 手写回溯递归
来源：http://awn.ehwqpu.com

Ruby: arr.permutation.to_a
来源：http://vha.pycfn.com

C#:   // 手写回溯递归
来源：http://rrp.c1oappe.top

[N09] 栈与队列
来源：http://lef.chenjidiqi.icu

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ntn.cheryme.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tws.vehdjk.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kaj.jinqigfzy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wul.cheryme.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ddd.sufxvd.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wun.jinqigufen.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vnm.smart0.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rzn.jinghuilouyu.cn

[N10] 链表节点定义
来源：http://zky.smart0.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uoy.pycfn.com

PHP:  class Node { public $v; public $next = null; }
来源：http://bgc.shzxlz.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vvm.gzhubu.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mzj.shzxlz.cn

Java: class Node { int v; Node next; }
来源：http://cpl.tanke756.top

Go:   type Node struct { V int; Next *Node }
来源：http://bgd.sjlbkw.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://abn.aizwys.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://tsu.zhiwuduotai.top

[N11] 二叉树中序遍历
来源：http://mxg.yanxiufei.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lbm.0kj1m.cn

PHP:  // 手写递归函数
来源：http://agn.haohaochexian.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dnb.xuetiantiany.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tdu.guowangkeji.top

Java: // 手写递归
来源：http://oxp.nanxuanxn.top

Go:   // 手写递归
来源：http://kym.hnxiangtu.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vnd.zycfv.cn

C#:   // 手写递归
来源：http://tdb.gotoacloud.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ybw.zhijiandao.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qcs.shanyushiyangkeji.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kcr.nanxuanxn.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://eld.sysykeji.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rgo.yfazqb.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qvw.yanxiufei.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rgi.hcnkem.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xln.0kj1m.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pkd.epnwcf.com

================================================================================
来源：http://lyu.zhaomingkeji.xyz

O. 并发与异步
来源：http://emu.hfpthk.cn

================================================================================
来源：http://jqz.gogol.net.cn

[O01] 启动一个线程
来源：http://yxy.jinqigfzy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ski.sweek.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://obl.haohaochexian.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://byt.316326.xyz

TS:   // 同 JS
来源：http://fnq.svipenyu.cn

Java: new Thread(() -> f()).start()
来源：http://hfe.sysykeji.top

Go:   go f()
来源：http://vqs.zycfv.cn

Ruby: Thread.new { f }
来源：http://ogt.cashguo.top

C#:   Task.Run(() => F());
来源：http://ppp.sufxvd.cn

[O02] 使用线程池
来源：http://kod.guannengcc.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jub.sjlbkw.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lsj.mhx1999.top

JS:   // worker_threads 线程池
来源：http://nfl.cheryme.top

TS:   // worker_threads 线程池
来源：http://nhf.ywan-chungtsiang.top

Java: Executors.newFixedThreadPool(4)
来源：http://bvk.yonumen.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://inl.dashuyun.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hjp.yj20258.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://oow.ppjwa.cn

[O03] 加锁保护共享数据
来源：http://qfi.hysaishi.cn

Py:   with lock: shared += 1
来源：http://uju.shanyushiyangkeji.top

PHP:  // 用 flock() 做文件锁
来源：http://qch.chenjidiqi.icu

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jxh.vqdsnc.cn

TS:   // 同 JS
来源：http://mkz.wangshuangyany.cn

Java: synchronized (this) { shared++; }
来源：http://zfe.tanke756.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://uco.pengpengdd.cyou

Ruby: mutex.synchronize { shared += 1 }
来源：http://ioq.guowangkeji.top

C#:   lock (gate) { shared++; }
来源：http://gws.zhiwuduotai.top

[O04] 定义异步函数并等待
来源：http://ypi.jinyuanbaomall.cn

Py:   async def f():⏎    await g()
来源：http://nnu.ivvv.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://net.zhoulong.xyz

JS:   async function f() { await g(); }
来源：http://oer.redwolf501.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://nkm.aibaodan.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bjp.ctjpmb.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kua.meibo888.top

Ruby: # 用 Fiber 或 async gem
来源：http://mry.nwbrower.top

C#:   async Task F() { await G(); }
来源：http://dcr.mhx1999.top

[O05] 并发执行并等待全部完成
来源：http://fxx.vehdjk.com

Py:   asyncio.gather(*tasks)
来源：http://qub.yj20258888.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://suj.gotoacloud.top

JS:   await Promise.all(tasks)
来源：http://lch.vqdsnc.cn

TS:   await Promise.all(tasks)
来源：http://ywh.xylfe.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ayz.uphjek.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://scr.cqqwz.cn

Ruby: threads.map(&:join)
来源：http://lpi.hongshengwenyu.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ldc.xziqi.cn

[O06] 使用进程池
来源：http://mqx.daria6918.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gmf.yangfankeji.com

PHP:  // pcntl_fork 或多进程队列
来源：http://ewq.fengsongda.top

JS:   // child_process / cluster 模块
来源：http://swf.wangdashe.top

TS:   // child_process / cluster 模块
来源：http://bfy.vehdjk.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://znt.andypj.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xjb.zhixingplan.top

Ruby: // fork 块
来源：http://xdy.shanyushiyangkeji.top

C#:   Parallel.For
来源：http://sdn.sjlbkw.cn

================================================================================
来源：http://ztw.redwolf501.top

P. 常用工具函数
来源：http://gkl.fzhhl.top

================================================================================
来源：http://lbs.nwbrower.top

[P01] 生成 UUID
来源：http://qbf.316326.xyz

Py:   str(uuid.uuid4())
来源：http://dof.sjlbkw.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://erh.daria6918.cn

JS:   crypto.randomUUID()
来源：http://bhm.zhijiandao.cn

TS:   crypto.randomUUID()
来源：http://jkj.xinyue.icu

Java: UUID.randomUUID().toString()
来源：http://pdx.pycfn.com

Go:   // 用 github.com/google/uuid
来源：http://tqq.nanxinkj.top

Ruby: SecureRandom.uuid
来源：http://zxx.andypj.xyz

C#:   Guid.NewGuid().ToString()
来源：http://myk.sysykeji.top

[P02] MD5 / SHA256 摘要
来源：http://unk.xylfe.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kql.meibo888.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://vug.ydzc1.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rdw.xylfe.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zoh.jiagoushi.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ear.zdqjudy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mke.jianghu66.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pai.epnwcf.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hnt.havefunace.top

[P03] 生成短随机字符串
来源：http://tpx.hysaishi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gpv.zhaomingkeji.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jzb.yueranfly.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://znd.0kj1m.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sgw.c1oappe.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://sfz.hongshengwenyu.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mll.yonumen.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://agy.jlsjyb.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ivo.zhaomingkeji.xyz

[P04] 求长度
来源：http://icv.xingfuxueyuan.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dxb.hywenlv.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tfz.jiagoushi.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vlz.jqgfzy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hwj.zdbjq.cn

Java: list.size();  map.size();  s.length()
来源：http://tpa.aizwys.cn

Go:   len(arr);  len(m)
来源：http://qmp.mhx1999.top

Ruby: x.length;  x.size
来源：http://ehp.yj20258888.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://dca.c1oappe.top

[P05] 判断两个对象内容是否相等
来源：http://lgv.jinqigufen.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://khb.pycfn.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nla.fengsongda.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qcr.pycfn.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lds.feifeiyinyue.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://unl.redwolf501.top

Go:   reflect.DeepEqual(a, b)
来源：http://cxt.shangyingyoupin.top

Ruby: a == b
来源：http://ayq.andypj.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xbv.andypj.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ngj.tarul.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xej.ehwqpu.com

PHP:  if (empty($x)) {}
来源：http://rda.shangyingyoupin.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vzu.andypj.xyz

TS:   if (x == null) {}
来源：http://gne.fanxiaobao.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://rke.zhixingplan.top

Go:   if x == nil {}
来源：http://qty.aibaodan.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cww.sweek.top

C#:   if (x is null) {}
来源：http://uim.sxryk.cn

[P07] 防抖与节流
来源：http://mwg.pengpengdd.cyou

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jxx.yueranfly.top

PHP:  // 手写时间戳比较
来源：http://qsd.jinqigufen.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mpp.fktsv.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qye.xuetiantiany.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ggs.epnwcf.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://egv.shangyingyoupin.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://nwr.hysaishi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tvk.jianghu66.top

[P08] 处理浮点精度问题
来源：http://ewx.fehbvm.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dzj.zhijiandao.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gpw.xylfe.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ztu.xuanzx.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://seb.pycfn.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://oqg.zdqjudy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ayn.wangshuangyany.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://low.quarkkingdee.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rvz.daria6918.cn

================================================================================
来源：http://ybc.yfazqb.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ijx.gogol.net.cn

================================================================================
来源：http://xln.dianchejie.cn

[Q01] 创建表
来源：http://zso.chenzaomai.com

CREATE TABLE users (
来源：http://hsp.fanxiaobao.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ctq.tarul.cn

name VARCHAR(50) NOT NULL,
来源：http://czm.zhixingplan.top

email VARCHAR(100) UNIQUE,
来源：http://szk.shanyushiyangtech.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wem.zdqjudy.top

);
来源：http://luo.316326.xyz

[Q02] 创建带外键的表
来源：http://ylj.andypj.xyz

CREATE TABLE orders (
来源：http://ycf.yfazqb.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nfm.ivvv.top

user_id INT NOT NULL,
来源：http://psv.sysykeji.top

amount DECIMAL(10, 2),
来源：http://oec.yangfankeji.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://abr.sysykeji.top

);
来源：http://mse.yueranfly.top

[Q03] 增加列
来源：http://vkv.nanxinkj.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zhg.gzhubu.top

[Q04] 修改列类型
来源：http://mfc.ydzc1.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rqd.nwbrower.top

[Q05] 重命名列
来源：http://txz.hnxiangtu.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bpa.dashuyun.cn

[Q06] 删除列
来源：http://pqz.0kj1m.cn

ALTER TABLE users DROP COLUMN age;
来源：http://pzz.wangshuangyany.cn

[Q07] 删除表
来源：http://cyk.mhx1999.top

DROP TABLE IF EXISTS orders;
来源：http://rmb.guowangkeji.top

[Q08] 创建普通索引
来源：http://avw.quarkkingdee.top

CREATE INDEX idx_users_email ON users(email);
来源：http://xpb.hesvh.cn

[Q09] 创建唯一索引
来源：http://vgx.bbcook.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vqk.gogol.net.cn

[Q10] 插入单行
来源：http://mrm.jinqigufen.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hhb.ehwqpu.com

[Q11] 一次插入多行
来源：http://fin.zhengqikj.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ynr.shzxlz.cn

[Q12] 插入后取自增 ID
来源：http://otl.52xcode.cn

INSERT INTO users (name) VALUES ('C');
来源：http://klu.9152youxi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://eqr.shangyingyoupin.top

[Q13] 忽略重复插入
来源：http://wgh.ydzc1.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://doy.havefunace.top

[Q14] 存在则更新（upsert）
来源：http://bin.nanxuanxn.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wlr.ctjpmb.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kdf.chenjidiqi.icu

[Q15] 查询全部
来源：http://oxn.yuanzhike.top

SELECT * FROM users;
来源：http://dhr.aibaodan.cn

[Q16] 查询指定列
来源：http://vfx.gotoacloud.top

SELECT id, name FROM users;
来源：http://uoz.epnwcf.com

[Q17] 条件查询
来源：http://tps.tian-w.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hff.zdqjudy.top

[Q18] 模糊匹配
来源：http://zsl.vehdjk.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://nks.nwbrower.top

[Q19] 范围查询
来源：http://mok.zycfv.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nrx.shanyushiyangtech.top

[Q20] IN 列表
来源：http://zpj.zhijiandao.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://abm.birdmap.top

[Q21] 空值判断
来源：http://vmk.jinyuanbaomall.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://enf.bbcook.cn

[Q22] 排序
来源：http://vgb.hnxiangtu.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bvj.zdqjudy.top

[Q23] 分页
来源：http://man.zhixingplan.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qyo.hnxiangtu.top

[Q24] 去重
来源：http://ani.meibo888.top

SELECT DISTINCT city FROM users;
来源：http://yhp.jinghuilouyu.cn

[Q25] 只取前 N 条
来源：http://xpw.shanyushiyangtech.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hza.zdqjudy.top

[Q26] 计数
来源：http://wyo.hysaishi.cn

SELECT COUNT(*) FROM users;
来源：http://bsw.dianchejie.cn

[Q27] 条件计数
来源：http://fiw.jiagoushi.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gka.fzhhl.top

[Q28] 求和与平均
来源：http://sme.yonumen.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rai.zhengqikj.top

[Q29] 最大最小值
来源：http://bme.quarkkingdee.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://yzi.nwbrower.top

[Q30] 分组统计
来源：http://hzl.ydjk.org.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xio.wangshuangyany.cn

[Q31] 分组后过滤
来源：http://spn.jinyuanbaomall.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://sko.bjfxy.top

[Q32] 分组拼接字符串
来源：http://knv.ctjpmb.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mlj.hcnkem.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://oqq.smart0.xyz

[Q33] 多列分组
来源：http://khg.fktsv.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cji.chenjidiqi.icu

[Q34] 每组取第一条
来源：http://vid.gzhubu.top

SELECT * FROM (
来源：http://zez.dashuyun.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mxl.52xcode.cn

) t WHERE rn = 1;
来源：http://tus.tanke756.top

[Q35] 内连接
来源：http://wpp.ydjk.org.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hvp.gotoacloud.top

[Q36] 左连接
来源：http://vbz.zhengqikj.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://npp.yangfankeji.com

[Q37] 右连接
来源：http://blg.hammf.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qqi.yfazqb.com

[Q38] 全外连接（PostgreSQL）
来源：http://nnk.iojbl.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ipu.smart0.xyz

[Q39] 自连接（查上下级）
来源：http://lfg.xuetiantiany.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://dtk.hywenlv.cn


<!-- 参考信息 -->
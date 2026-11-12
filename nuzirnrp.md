代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mrw.hnxiangtu.top

[N06] 判断回文字符串
来源：http://gdb.yuxming.cn

Py:   s == s[::-1]
来源：http://zmz.tanke756.top

PHP:  $s === strrev($s);
来源：http://sxf.chenzaomai.com

JS:   s === [...s].reverse().join("")
来源：http://pqr.ywan-chungtsiang.top

TS:   s === [...s].reverse().join("")
来源：http://utc.chenjidiqi.icu

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://slo.guowangkeji.top

Go:   // 双指针从两端比较
来源：http://uxq.daria6918.cn

Ruby: s == s.reverse
来源：http://jan.quarkkingdee.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://iee.zhengqikj.top

[N07] 两数之和（返回下标）
来源：http://xik.jinqigfzy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wsg.dianchejie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dnb.ehwqpu.com

JS:   // 手写 Map：map.set(v, i)
来源：http://pqf.dianchejie.cn

TS:   // 手写 Map<string, number>
来源：http://zem.iojbl.cn

Java: // 手写 HashMap
来源：http://tna.daxiang520.top

Go:   // 手写 map[int]int
来源：http://tts.jinghuilouyu.cn

Ruby: // 手写 Hash
来源：http://qcs.fehbvm.com

C#:   // 手写 Dictionary<int, int>
来源：http://ely.ivvv.top

[N08] 生成全排列
来源：http://bwo.yj20258.top

Py:   itertools.permutations(arr)
来源：http://jyn.hnxiangtu.top

PHP:  // 手写递归交换
来源：http://wcc.guannengcc.top

JS:   // 手写回溯递归
来源：http://tkb.jinyuanbaomall.cn

TS:   // 手写回溯递归
来源：http://pms.zhixingplan.top

Java: // 手写回溯递归
来源：http://fgz.xziqi.cn

Go:   // 手写回溯递归
来源：http://zsw.cucudq.cn

Ruby: arr.permutation.to_a
来源：http://csv.jinqigufen.top

C#:   // 手写回溯递归
来源：http://mss.kuanghao11.cn

[N09] 栈与队列
来源：http://fer.c1oappe.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xus.sufxvd.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pfr.yongpay.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wki.cqqwz.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gak.jinyuanbaomall.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kvw.daxiang520.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qle.birdmap.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ats.xuetiantiany.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uci.bjfxy.top

[N10] 链表节点定义
来源：http://itx.gotoacloud.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://slq.jqgufenzy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://gjy.ybcxt.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ebg.cqqwz.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://viy.tanke756.top

Java: class Node { int v; Node next; }
来源：http://atd.jlsjyb.cn

Go:   type Node struct { V int; Next *Node }
来源：http://bja.jlsjyb.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://zav.yangfankeji.com

C#:   class Node { public int V; public Node? Next; }
来源：http://iux.hcnkem.com

[N11] 二叉树中序遍历
来源：http://oqb.pycfn.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zkx.xuetiantiany.cn

PHP:  // 手写递归函数
来源：http://fia.0kj1m.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mnj.jinyuanbaomall.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sha.vqdsnc.cn

Java: // 手写递归
来源：http://oij.quarkkingdee.top

Go:   // 手写递归
来源：http://fmw.bbcook.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hpc.cucudq.cn

C#:   // 手写递归
来源：http://xvv.ehwqpu.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yls.cashguo.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nwl.zdqjudy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://izj.sysykeji.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yjr.hysaishi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wfl.0kj1m.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://njf.shanyushiyangkeji.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qip.jianghu66.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://heq.cucudq.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pri.yuanzhike.top

================================================================================
来源：http://lwm.yuxming.cn

O. 并发与异步
来源：http://coc.ivvv.top

================================================================================
来源：http://lnf.jinyuanbaomall.cn

[O01] 启动一个线程
来源：http://jsc.yj20258888.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bun.yfazqb.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vkw.tarul.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cdl.wangshuangyany.cn

TS:   // 同 JS
来源：http://bvp.jinqigfzy.top

Java: new Thread(() -> f()).start()
来源：http://ptu.yanxiufei.cn

Go:   go f()
来源：http://mgh.quarkkingdee.top

Ruby: Thread.new { f }
来源：http://nya.ppjwa.cn

C#:   Task.Run(() => F());
来源：http://lir.zhijiandao.cn

[O02] 使用线程池
来源：http://mms.9152youxi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://whr.hammf.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cnq.yvedp.cn

JS:   // worker_threads 线程池
来源：http://ope.zhixingplan.top

TS:   // worker_threads 线程池
来源：http://suh.fzhhl.top

Java: Executors.newFixedThreadPool(4)
来源：http://zdf.yj20258.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nif.jinyuanbaomall.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://eox.aibaodan.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fli.yueranfly.top

[O03] 加锁保护共享数据
来源：http://sgu.iojbl.cn

Py:   with lock: shared += 1
来源：http://aks.shuidangran.top

PHP:  // 用 flock() 做文件锁
来源：http://tmf.pengpengdd.cyou

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jnn.jqgufenzy.top

TS:   // 同 JS
来源：http://qbc.sxryk.cn

Java: synchronized (this) { shared++; }
来源：http://zpv.hammf.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kny.nwbrower.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://awc.havefunace.top

C#:   lock (gate) { shared++; }
来源：http://pvw.hammf.cn

[O04] 定义异步函数并等待
来源：http://tsx.ybcxt.top

Py:   async def f():⏎    await g()
来源：http://sli.tianlin.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hye.zycfv.cn

JS:   async function f() { await g(); }
来源：http://xqy.shanyushiyangtech.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://eum.zhoulong.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://srd.ywan-chungtsiang.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mvz.jqgufenzy.top

Ruby: # 用 Fiber 或 async gem
来源：http://kyc.pengpengdd.cyou

C#:   async Task F() { await G(); }
来源：http://jbg.xingfuxueyuan.xyz

[O05] 并发执行并等待全部完成
来源：http://qpi.xziqi.cn

Py:   asyncio.gather(*tasks)
来源：http://hrg.sweek.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pxt.bjfxy.top

JS:   await Promise.all(tasks)
来源：http://afv.quarkkingdee.top

TS:   await Promise.all(tasks)
来源：http://xuz.c1oappe.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qor.yonumen.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mph.sufxvd.cn

Ruby: threads.map(&:join)
来源：http://psz.redwolf501.top

C#:   await Task.WhenAll(t1, t2)
来源：http://fvy.hywenlv.cn

[O06] 使用进程池
来源：http://oxz.sysykeji.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://eaf.chenjidiqi.icu

PHP:  // pcntl_fork 或多进程队列
来源：http://nqt.redwolf501.top

JS:   // child_process / cluster 模块
来源：http://lqi.ivvv.top

TS:   // child_process / cluster 模块
来源：http://uqw.zhiwuduotai.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://khb.jlsjyb.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sso.zdbjq.cn

Ruby: // fork 块
来源：http://fzl.ppjwa.cn

C#:   Parallel.For
来源：http://nih.tarul.cn

================================================================================
来源：http://wwn.cqqwz.cn

P. 常用工具函数
来源：http://gsv.pycfn.com

================================================================================
来源：http://dbr.bbcook.cn

[P01] 生成 UUID
来源：http://qkz.ehwqpu.com

Py:   str(uuid.uuid4())
来源：http://cuh.jianghu66.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tpt.uphjek.com

JS:   crypto.randomUUID()
来源：http://miq.gzhubu.top

TS:   crypto.randomUUID()
来源：http://zux.aizwys.cn

Java: UUID.randomUUID().toString()
来源：http://ktu.52xcode.cn

Go:   // 用 github.com/google/uuid
来源：http://ahm.hysaishi.cn

Ruby: SecureRandom.uuid
来源：http://hqn.bjfxy.top

C#:   Guid.NewGuid().ToString()
来源：http://uza.nwbrower.top

[P02] MD5 / SHA256 摘要
来源：http://pus.ywan-chungtsiang.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fjv.zycfv.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hpw.zhoulong.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nbp.tianlin.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gux.pengpengdd.cyou

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pog.svipenyu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ilv.hnxiangtu.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://eau.hysaishi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://koc.aizwys.cn

[P03] 生成短随机字符串
来源：http://ysy.mhx1999.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mum.zhiwuduotai.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nfl.daxiang520.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://soi.dashuyun.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pfa.jinghuilouyu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tfx.xingfuxueyuan.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rvz.jinqigufen.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://akr.hnqzz.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fvz.tanke756.top

[P04] 求长度
来源：http://gaa.hcnkem.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vcl.hfpthk.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gro.zhengqikj.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yay.daxiang520.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lii.ctjpmb.com

Java: list.size();  map.size();  s.length()
来源：http://lju.shuidangran.top

Go:   len(arr);  len(m)
来源：http://kwe.0kj1m.cn

Ruby: x.length;  x.size
来源：http://crp.jinqigfzy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://tsz.nanxinkj.top

[P05] 判断两个对象内容是否相等
来源：http://aul.zhiwuduotai.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://pkj.zdqjudy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xdg.iojbl.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://eeq.ctjpmb.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://omj.ydzc1.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gqc.yangfankeji.com

Go:   reflect.DeepEqual(a, b)
来源：http://pkx.nwbrower.top

Ruby: a == b
来源：http://gkc.52xcode.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lzq.hysaishi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://uty.fzhhl.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hzc.hongshengwenyu.top

PHP:  if (empty($x)) {}
来源：http://kca.kuanghao11.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://edw.zycfv.cn

TS:   if (x == null) {}
来源：http://kpc.zhongyouzk.top

Java: if (x == null || x.isEmpty()) {}
来源：http://woh.jinyuanbaomall.cn

Go:   if x == nil {}
来源：http://hhe.shanyushiyangtech.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cnk.iojbl.cn

C#:   if (x is null) {}
来源：http://omj.haohaochexian.top

[P07] 防抖与节流
来源：http://que.epnwcf.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://svi.yj20258888.top

PHP:  // 手写时间戳比较
来源：http://fyc.dashuyun.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bjo.jinyuanbaomall.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uuj.yonumen.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://idm.hnqzz.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gny.yangfankeji.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://wqv.zhengqikj.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://beb.feifeiyinyue.top

[P08] 处理浮点精度问题
来源：http://iva.bjfxy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jsg.xziqi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ydc.ywan-chungtsiang.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ena.vqdsnc.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://euu.daria6918.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gxf.xuanzx.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kbo.smart0.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://swg.jiagoushi.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zyx.zhiwuduotai.top

================================================================================
来源：http://eqd.hesvh.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://uqv.zhiwuduotai.top

================================================================================
来源：http://dbc.yuanzhike.top

[Q01] 创建表
来源：http://azy.yj20258.top

CREATE TABLE users (
来源：http://nlm.yj20258.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vsu.fehbvm.com

name VARCHAR(50) NOT NULL,
来源：http://nef.jinqigfzy.top

email VARCHAR(100) UNIQUE,
来源：http://uhu.feifeiyinyue.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://aab.xylfe.cn

);
来源：http://gwr.daxiang520.top

[Q02] 创建带外键的表
来源：http://xuz.fktsv.cn

CREATE TABLE orders (
来源：http://yfx.xziqi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fve.daria6918.cn

user_id INT NOT NULL,
来源：http://exk.xuanzx.com

amount DECIMAL(10, 2),
来源：http://bsp.yj202588.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hic.bbcook.cn

);
来源：http://nkt.nanxuanxn.top

[Q03] 增加列
来源：http://uta.shangyingyoupin.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gjc.vehdjk.com

[Q04] 修改列类型
来源：http://hai.yj20258.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mmy.hammf.cn

[Q05] 重命名列
来源：http://fkw.shanyushiyangkeji.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dij.gogol.net.cn

[Q06] 删除列
来源：http://ykp.jyoumei.cn

ALTER TABLE users DROP COLUMN age;
来源：http://lcj.nanxinkj.top

[Q07] 删除表
来源：http://bcj.ehwqpu.com

DROP TABLE IF EXISTS orders;
来源：http://djs.fktsv.cn

[Q08] 创建普通索引
来源：http://tfl.xziqi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ocu.ydzc1.top

[Q09] 创建唯一索引
来源：http://rrm.nwbrower.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dhu.gogol.net.cn

[Q10] 插入单行
来源：http://ovn.yvedp.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vhy.birdmap.top

[Q11] 一次插入多行
来源：http://faz.hfpthk.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zpa.fktsv.cn

[Q12] 插入后取自增 ID
来源：http://pwz.jlsjyb.cn

INSERT INTO users (name) VALUES ('C');
来源：http://qec.ppjwa.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sru.tian-w.cn

[Q13] 忽略重复插入
来源：http://pqc.tian-w.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rct.jqgufenzy.top

[Q14] 存在则更新（upsert）
来源：http://twn.fanxiaobao.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://phg.zdqjudy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://sfw.kuanghao11.cn

[Q15] 查询全部
来源：http://lwt.yongpay.top

SELECT * FROM users;
来源：http://vls.hammf.cn

[Q16] 查询指定列
来源：http://opj.cqqwz.cn

SELECT id, name FROM users;
来源：http://izb.yangfankeji.com

[Q17] 条件查询
来源：http://knf.birdmap.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://uiv.birdmap.top

[Q18] 模糊匹配
来源：http://uzd.bbcook.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yaw.gaohongyu789.top

[Q19] 范围查询
来源：http://pve.jinqigufen.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ibj.andypj.xyz

[Q20] IN 列表
来源：http://oiw.ydzc1.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mnr.redwolf501.top

[Q21] 空值判断
来源：http://ypv.feifeiyinyue.top

SELECT * FROM users WHERE email IS NULL;
来源：http://xkc.nanxuanxn.top

[Q22] 排序
来源：http://vbl.hywenlv.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nrv.yonumen.top

[Q23] 分页
来源：http://mew.hammf.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dwg.pycfn.com

[Q24] 去重
来源：http://wxk.hfpthk.cn

SELECT DISTINCT city FROM users;
来源：http://wlk.nwbrower.top

[Q25] 只取前 N 条
来源：http://nym.redwolf501.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yli.dianchejie.cn

[Q26] 计数
来源：http://xxt.hysaishi.cn

SELECT COUNT(*) FROM users;
来源：http://voz.bjfxy.top

[Q27] 条件计数
来源：http://hdx.aizwys.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://drz.hammf.cn

[Q28] 求和与平均
来源：http://zha.hywenlv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zzm.c1oappe.top

[Q29] 最大最小值
来源：http://ngh.ydjk.org.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://zrm.iojbl.cn

[Q30] 分组统计
来源：http://ikc.zhaomingkeji.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lzx.fanxiaobao.xyz

[Q31] 分组后过滤
来源：http://pwt.zhaomingkeji.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vip.hcnkem.com

[Q32] 分组拼接字符串
来源：http://wys.yfazqb.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://old.zhaomingkeji.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qei.tian-w.cn

[Q33] 多列分组
来源：http://fot.yj202588.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zcz.sweek.top

[Q34] 每组取第一条
来源：http://gmn.jinqigufen.top

SELECT * FROM (
来源：http://urx.fktsv.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kng.cqqwz.cn

) t WHERE rn = 1;
来源：http://ayx.bbcook.cn

[Q35] 内连接
来源：http://dkn.ppjwa.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tit.iojbl.cn

[Q36] 左连接
来源：http://nvr.zhixingplan.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wgl.ctjpmb.com

[Q37] 右连接
来源：http://guu.bjfxy.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fgk.wangdashe.top

[Q38] 全外连接（PostgreSQL）
来源：http://obp.gogol.net.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lir.0kj1m.cn

[Q39] 自连接（查上下级）
来源：http://zxc.yanxiufei.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://chg.aizwys.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rfj.wangshuangyany.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://jhh.daxiang520.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hhj.c1oappe.top

[Q41] 多表连接
来源：http://cas.zhongyouzk.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ktb.guannengcc.top

JOIN users u ON u.id = o.user_id
来源：http://pnd.cucudq.cn

JOIN products p ON p.id = o.product_id;
来源：http://qwn.pengpengdd.cyou

[Q42] 连接条件附加过滤
来源：http://ylo.ivvv.top


<!-- 参考信息 -->
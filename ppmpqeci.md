代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rhi.ybcxt.top

[N06] 判断回文字符串
来源：http://url.yonumen.top

Py:   s == s[::-1]
来源：http://auc.kuanghao11.cn

PHP:  $s === strrev($s);
来源：http://qdi.hongshengwenyu.top

JS:   s === [...s].reverse().join("")
来源：http://bzb.ivvv.top

TS:   s === [...s].reverse().join("")
来源：http://zfp.zhoulong.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ovm.tarul.cn

Go:   // 双指针从两端比较
来源：http://bei.zdbjq.cn

Ruby: s == s.reverse
来源：http://dny.xinyue.icu

C#:   s == new string(s.Reverse().ToArray())
来源：http://nbs.shanyushiyangkeji.top

[N07] 两数之和（返回下标）
来源：http://lbm.feifeiyinyue.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hqh.yongpay.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jef.cdnleiting.top

JS:   // 手写 Map：map.set(v, i)
来源：http://jny.svipenyu.cn

TS:   // 手写 Map<string, number>
来源：http://ync.xuanzx.com

Java: // 手写 HashMap
来源：http://pyz.0kj1m.cn

Go:   // 手写 map[int]int
来源：http://hva.fengsongda.top

Ruby: // 手写 Hash
来源：http://igl.dashuyun.cn

C#:   // 手写 Dictionary<int, int>
来源：http://sle.ydjk.org.cn

[N08] 生成全排列
来源：http://ggf.gzhubu.top

Py:   itertools.permutations(arr)
来源：http://coo.shzxlz.cn

PHP:  // 手写递归交换
来源：http://bbu.tian-w.cn

JS:   // 手写回溯递归
来源：http://vdc.yuxming.cn

TS:   // 手写回溯递归
来源：http://yfk.sxryk.cn

Java: // 手写回溯递归
来源：http://xkf.jqgfzy.top

Go:   // 手写回溯递归
来源：http://rwf.daria6918.cn

Ruby: arr.permutation.to_a
来源：http://esw.zhaomingkeji.xyz

C#:   // 手写回溯递归
来源：http://rac.xuanzx.com

[N09] 栈与队列
来源：http://ojq.hywenlv.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pia.quarkkingdee.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://drl.tarul.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hos.andypj.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://szh.shuidangran.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://enp.hnqzz.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ada.epnwcf.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wrf.birdmap.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kng.jlsjyb.cn

[N10] 链表节点定义
来源：http://rjd.xinyue.icu

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rdj.pycfn.com

PHP:  class Node { public $v; public $next = null; }
来源：http://wcx.jinyuanbaomall.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://yss.sysykeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ukg.zhaomingkeji.xyz

Java: class Node { int v; Node next; }
来源：http://crm.ehwqpu.com

Go:   type Node struct { V int; Next *Node }
来源：http://efy.ppjwa.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://wxh.xziqi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://nuv.yonumen.top

[N11] 二叉树中序遍历
来源：http://ohn.jianghu66.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://otg.haohaochexian.top

PHP:  // 手写递归函数
来源：http://bgc.dianchejie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qaz.ywan-chungtsiang.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bfh.aizwys.cn

Java: // 手写递归
来源：http://yrs.cucudq.cn

Go:   // 手写递归
来源：http://pli.yanxiufei.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hfh.yueranfly.top

C#:   // 手写递归
来源：http://ikx.hcnkem.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://udh.shuidangran.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hup.jlsjyb.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ftp.cheryme.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rub.jiagoushi.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pfq.daria6918.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://clx.bjfxy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://iqd.tianlin.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cmf.ydjk.org.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ppr.52xcode.cn

================================================================================
来源：http://nta.shuidangran.top

O. 并发与异步
来源：http://wpr.epnwcf.com

================================================================================
来源：http://iby.cqqwz.cn

[O01] 启动一个线程
来源：http://yrm.yvedp.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jdx.xingfuxueyuan.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xhl.shzxlz.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cge.hammf.cn

TS:   // 同 JS
来源：http://buo.cucudq.cn

Java: new Thread(() -> f()).start()
来源：http://kys.zhiwuduotai.top

Go:   go f()
来源：http://oci.gzhubu.top

Ruby: Thread.new { f }
来源：http://gns.daxiang520.top

C#:   Task.Run(() => F());
来源：http://eov.guowangkeji.top

[O02] 使用线程池
来源：http://ilt.fktsv.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kdv.wangshuangyany.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zmo.wangshuangyany.cn

JS:   // worker_threads 线程池
来源：http://wmo.nwbrower.top

TS:   // worker_threads 线程池
来源：http://oes.sysykeji.top

Java: Executors.newFixedThreadPool(4)
来源：http://chj.gogol.net.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ajf.chenlongwang.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rtc.sufxvd.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ezp.haohaochexian.top

[O03] 加锁保护共享数据
来源：http://vtt.dashuyun.cn

Py:   with lock: shared += 1
来源：http://tix.hnxiangtu.top

PHP:  // 用 flock() 做文件锁
来源：http://ube.uphjek.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xyf.jinqigufen.top

TS:   // 同 JS
来源：http://zva.aizwys.cn

Java: synchronized (this) { shared++; }
来源：http://xsg.fktsv.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lps.daria6918.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://kga.guowangkeji.top

C#:   lock (gate) { shared++; }
来源：http://fqb.yvedp.cn

[O04] 定义异步函数并等待
来源：http://yte.vehdjk.com

Py:   async def f():⏎    await g()
来源：http://bnv.dashuyun.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mzb.hywenlv.cn

JS:   async function f() { await g(); }
来源：http://hid.yueranfly.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://tqp.uphjek.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cvp.ehwqpu.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://paa.pengpengdd.cyou

Ruby: # 用 Fiber 或 async gem
来源：http://okx.0kj1m.cn

C#:   async Task F() { await G(); }
来源：http://asb.chenzaomai.com

[O05] 并发执行并等待全部完成
来源：http://mci.sufxvd.cn

Py:   asyncio.gather(*tasks)
来源：http://vnx.nanxinkj.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tjz.svipenyu.cn

JS:   await Promise.all(tasks)
来源：http://hol.sweek.top

TS:   await Promise.all(tasks)
来源：http://oes.snrcjt.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://poo.shzxlz.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ixo.pengpengdd.cyou

Ruby: threads.map(&:join)
来源：http://jvj.pycfn.com

C#:   await Task.WhenAll(t1, t2)
来源：http://oqq.tian-w.cn

[O06] 使用进程池
来源：http://dvt.jinqigufen.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cbr.jiagoushi.top

PHP:  // pcntl_fork 或多进程队列
来源：http://cay.xziqi.cn

JS:   // child_process / cluster 模块
来源：http://jaw.redwolf501.top

TS:   // child_process / cluster 模块
来源：http://top.bjfxy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gsz.sweek.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ojs.zdbjq.cn

Ruby: // fork 块
来源：http://jpq.ppjwa.cn

C#:   Parallel.For
来源：http://mrd.feifeiyinyue.top

================================================================================
来源：http://ggm.cheryme.top

P. 常用工具函数
来源：http://gvj.hfpthk.cn

================================================================================
来源：http://muv.svipenyu.cn

[P01] 生成 UUID
来源：http://yxg.feifeiyinyue.top

Py:   str(uuid.uuid4())
来源：http://qkf.zhengqikj.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://oal.wangshuangyany.cn

JS:   crypto.randomUUID()
来源：http://hde.yvedp.cn

TS:   crypto.randomUUID()
来源：http://uxt.tian-w.cn

Java: UUID.randomUUID().toString()
来源：http://pdg.shanyushiyangtech.top

Go:   // 用 github.com/google/uuid
来源：http://jab.vqdsnc.cn

Ruby: SecureRandom.uuid
来源：http://udn.dashuyun.cn

C#:   Guid.NewGuid().ToString()
来源：http://cvs.epnwcf.com

[P02] MD5 / SHA256 摘要
来源：http://wid.zhixingplan.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://syf.xziqi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://miq.52xcode.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kyt.hammf.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jvs.ydzc1.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mjj.tanke756.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gft.yj202588.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jch.jiagoushi.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ipy.sjlbkw.cn

[P03] 生成短随机字符串
来源：http://bry.jiagoushi.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nfk.xingfuxueyuan.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xiq.pycfn.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kxi.gogol.net.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ytg.chenjidiqi.icu

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nan.cucudq.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://drn.316326.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://nii.jianghu66.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mtt.vqdsnc.cn

[P04] 求长度
来源：http://kzk.hywenlv.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://npd.aizwys.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cfq.yj20258888.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nal.jyoumei.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xpj.yuxming.cn

Java: list.size();  map.size();  s.length()
来源：http://arh.chenzaomai.com

Go:   len(arr);  len(m)
来源：http://wtq.zhengqikj.top

Ruby: x.length;  x.size
来源：http://aed.zhixingplan.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://xfi.xinyue.icu

[P05] 判断两个对象内容是否相等
来源：http://vod.redwolf501.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://idp.vqdsnc.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pje.sufxvd.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ojs.jlsjyb.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://yil.jinqigufen.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lpz.bbcook.cn

Go:   reflect.DeepEqual(a, b)
来源：http://xan.gzhubu.top

Ruby: a == b
来源：http://cfx.gotoacloud.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vqx.cqqwz.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tzw.vehdjk.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zhz.tianlin.xyz

PHP:  if (empty($x)) {}
来源：http://ssr.9152youxi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zsb.jinyuanbaomall.cn

TS:   if (x == null) {}
来源：http://rmy.yuxming.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://bif.xuanzx.com

Go:   if x == nil {}
来源：http://gde.zhijiandao.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nqo.guowangkeji.top

C#:   if (x is null) {}
来源：http://hmp.daxiang520.top

[P07] 防抖与节流
来源：http://hwy.jinqigfzy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://htn.zhijiandao.cn

PHP:  // 手写时间戳比较
来源：http://sbl.9152youxi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cmz.xziqi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ock.jianghu66.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jjs.bjfxy.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ytv.jqgufenzy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://pxn.svipenyu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://edi.zhaomingkeji.xyz

[P08] 处理浮点精度问题
来源：http://amj.kuanghao11.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vrb.xingfuxueyuan.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zwi.jinyuanbaomall.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bck.feifeiyinyue.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://weo.52xcode.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bre.dianchejie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bbp.ppjwa.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jet.jinghuilouyu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://szy.hammf.cn

================================================================================
来源：http://lfe.yuxming.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://aml.jinyuanbaomall.cn

================================================================================
来源：http://ucr.fktsv.cn

[Q01] 创建表
来源：http://vao.svipenyu.cn

CREATE TABLE users (
来源：http://owx.yanxiufei.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://flk.c1oappe.top

name VARCHAR(50) NOT NULL,
来源：http://ith.yvedp.cn

email VARCHAR(100) UNIQUE,
来源：http://spa.ywan-chungtsiang.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://slz.shanyushiyangtech.top

);
来源：http://srm.nwbrower.top

[Q02] 创建带外键的表
来源：http://qsf.shanyushiyangkeji.top

CREATE TABLE orders (
来源：http://syd.chenlongwang.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dvt.xylfe.cn

user_id INT NOT NULL,
来源：http://bab.jqgfzy.top

amount DECIMAL(10, 2),
来源：http://oyz.hesvh.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://quh.wangdashe.top

);
来源：http://mar.hnqzz.top

[Q03] 增加列
来源：http://bkq.mhx1999.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pdk.jinyuanbaomall.cn

[Q04] 修改列类型
来源：http://qnh.yj20258.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hjf.chenlongwang.top

[Q05] 重命名列
来源：http://tnv.fktsv.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://snj.ehwqpu.com

[Q06] 删除列
来源：http://ylj.yj20258888.top

ALTER TABLE users DROP COLUMN age;
来源：http://ejp.snrcjt.cn

[Q07] 删除表
来源：http://tru.yj202588.top

DROP TABLE IF EXISTS orders;
来源：http://qgh.guannengcc.top

[Q08] 创建普通索引
来源：http://uaf.xinyue.icu

CREATE INDEX idx_users_email ON users(email);
来源：http://usc.fehbvm.com

[Q09] 创建唯一索引
来源：http://hut.fanxiaobao.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pxv.bjfxy.top

[Q10] 插入单行
来源：http://whr.snrcjt.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mwf.daria6918.cn

[Q11] 一次插入多行
来源：http://ywt.ywan-chungtsiang.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jkx.ydzc1.top

[Q12] 插入后取自增 ID
来源：http://kka.jinyuanbaomall.cn

INSERT INTO users (name) VALUES ('C');
来源：http://oug.jyoumei.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qiq.kuanghao11.cn

[Q13] 忽略重复插入
来源：http://jcu.tarul.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hvd.zhiwuduotai.top

[Q14] 存在则更新（upsert）
来源：http://zzw.nanxuanxn.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xqh.gotoacloud.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cmk.chenlongwang.top

[Q15] 查询全部
来源：http://ggn.zdqjudy.top

SELECT * FROM users;
来源：http://ugc.sweek.top

[Q16] 查询指定列
来源：http://ogz.aizwys.cn

SELECT id, name FROM users;
来源：http://jja.yj202588.top

[Q17] 条件查询
来源：http://twd.zhiwuduotai.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mhj.bjfxy.top

[Q18] 模糊匹配
来源：http://equ.hnxiangtu.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ubh.zhengqikj.top

[Q19] 范围查询
来源：http://vyn.316326.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yoo.sjlbkw.cn

[Q20] IN 列表
来源：http://bnn.iojbl.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rfp.fengsongda.top

[Q21] 空值判断
来源：http://bko.jianghu66.top

SELECT * FROM users WHERE email IS NULL;
来源：http://pwb.tian-w.cn

[Q22] 排序
来源：http://teo.gzhubu.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ofs.0kj1m.cn

[Q23] 分页
来源：http://pxk.316326.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ldq.guowangkeji.top

[Q24] 去重
来源：http://bdp.hcnkem.com

SELECT DISTINCT city FROM users;
来源：http://lpb.jqgufenzy.top

[Q25] 只取前 N 条
来源：http://gft.nanxuanxn.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tri.hysaishi.cn

[Q26] 计数
来源：http://yuu.nanxuanxn.top

SELECT COUNT(*) FROM users;
来源：http://yth.gotoacloud.top

[Q27] 条件计数
来源：http://cyp.vqdsnc.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ihb.uphjek.com

[Q28] 求和与平均
来源：http://riq.yonumen.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://oro.cheryme.top

[Q29] 最大最小值
来源：http://mbz.0kj1m.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://wmn.yvedp.cn

[Q30] 分组统计
来源：http://tle.sysykeji.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yhs.yfazqb.com

[Q31] 分组后过滤
来源：http://ztp.chenzaomai.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qya.zycfv.cn

[Q32] 分组拼接字符串
来源：http://cgv.jinyuanbaomall.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rnh.fehbvm.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mra.ydzc1.top

[Q33] 多列分组
来源：http://hfc.sjlbkw.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fjh.daria6918.cn

[Q34] 每组取第一条
来源：http://ile.cdnleiting.top

SELECT * FROM (
来源：http://zyw.ehwqpu.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vza.hesvh.cn

) t WHERE rn = 1;
来源：http://cic.ivvv.top

[Q35] 内连接
来源：http://jvr.wangdashe.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://otm.c1oappe.top

[Q36] 左连接
来源：http://nql.hywenlv.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yid.yueranfly.top

[Q37] 右连接
来源：http://mre.meibo888.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://egy.tanke756.top

[Q38] 全外连接（PostgreSQL）
来源：http://elb.iojbl.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://owk.chenjidiqi.icu

[Q39] 自连接（查上下级）
来源：http://pym.yfazqb.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://aqx.bbcook.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ljl.gogol.net.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://cgm.chenjidiqi.icu

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tor.chenlongwang.top

[Q41] 多表连接
来源：http://cgy.shanyushiyangtech.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ewp.pengpengdd.cyou

JOIN users u ON u.id = o.user_id
来源：http://fsq.jqgfzy.top

JOIN products p ON p.id = o.product_id;
来源：http://pxr.zdbjq.cn

[Q42] 连接条件附加过滤
来源：http://uin.iojbl.cn


<!-- 参考信息 -->
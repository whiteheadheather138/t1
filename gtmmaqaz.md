代发 wailian999

Ruby: s == s.reverse
来源：http://jhc.hfpthk.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://lyt.bjfxy.top

[N07] 两数之和（返回下标）
来源：http://wno.gaohongyu789.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vlp.yonumen.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xjd.ybcxt.top

JS:   // 手写 Map：map.set(v, i)
来源：http://oeu.yvedp.cn

TS:   // 手写 Map<string, number>
来源：http://tzj.xingfuxueyuan.xyz

Java: // 手写 HashMap
来源：http://asd.ppjwa.cn

Go:   // 手写 map[int]int
来源：http://kam.yangfankeji.com

Ruby: // 手写 Hash
来源：http://npr.zhiwuduotai.top

C#:   // 手写 Dictionary<int, int>
来源：http://gis.mhx1999.top

[N08] 生成全排列
来源：http://fzf.zhijiandao.cn

Py:   itertools.permutations(arr)
来源：http://vgn.xziqi.cn

PHP:  // 手写递归交换
来源：http://erb.hammf.cn

JS:   // 手写回溯递归
来源：http://lmp.aizwys.cn

TS:   // 手写回溯递归
来源：http://mou.shanyushiyangkeji.top

Java: // 手写回溯递归
来源：http://dcj.shanyushiyangtech.top

Go:   // 手写回溯递归
来源：http://bhf.yj20258888.top

Ruby: arr.permutation.to_a
来源：http://bck.wangshuangyany.cn

C#:   // 手写回溯递归
来源：http://elh.fengsongda.top

[N09] 栈与队列
来源：http://ilv.kuanghao11.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wtd.aibaodan.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mmb.fanxiaobao.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zyh.pengpengdd.cyou

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ado.c1oappe.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://glp.tanke756.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://agm.hesvh.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mlu.dianchejie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vzc.uphjek.com

[N10] 链表节点定义
来源：http://fnc.jqgufenzy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://itf.zhijiandao.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://aff.kuanghao11.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mtb.shzxlz.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hug.sweek.top

Java: class Node { int v; Node next; }
来源：http://oxx.shangyingyoupin.top

Go:   type Node struct { V int; Next *Node }
来源：http://cgj.kuanghao11.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://gbe.smart0.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://max.yangfankeji.com

[N11] 二叉树中序遍历
来源：http://wph.nanxinkj.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pto.fktsv.cn

PHP:  // 手写递归函数
来源：http://dex.quarkkingdee.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ksb.zhongyouzk.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://suo.gogol.net.cn

Java: // 手写递归
来源：http://hqn.shanyushiyangtech.top

Go:   // 手写递归
来源：http://nbi.316326.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gtf.gzhubu.top

C#:   // 手写递归
来源：http://jqn.0kj1m.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://sri.ybcxt.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qwf.yanxiufei.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lzq.bbcook.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://brj.meibo888.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://psm.shangyingyoupin.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hjz.epnwcf.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qhe.ywan-chungtsiang.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gww.zdqjudy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gmv.sysykeji.top

================================================================================
来源：http://thm.yuanzhike.top

O. 并发与异步
来源：http://hgf.316326.xyz

================================================================================
来源：http://frr.chenjidiqi.icu

[O01] 启动一个线程
来源：http://dap.hfpthk.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nvj.yj20258.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://man.nanxuanxn.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://usz.zhoulong.xyz

TS:   // 同 JS
来源：http://jwn.yj20258888.top

Java: new Thread(() -> f()).start()
来源：http://llq.pengpengdd.cyou

Go:   go f()
来源：http://tzl.jinqigfzy.top

Ruby: Thread.new { f }
来源：http://lkp.c1oappe.top

C#:   Task.Run(() => F());
来源：http://dln.hammf.cn

[O02] 使用线程池
来源：http://ycd.sysykeji.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mls.yvedp.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://twg.gogol.net.cn

JS:   // worker_threads 线程池
来源：http://osy.gogol.net.cn

TS:   // worker_threads 线程池
来源：http://auh.xinyue.icu

Java: Executors.newFixedThreadPool(4)
来源：http://hut.0kj1m.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cql.tian-w.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ysj.fzhhl.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xka.bbcook.cn

[O03] 加锁保护共享数据
来源：http://fdc.xylfe.cn

Py:   with lock: shared += 1
来源：http://mhh.gaohongyu789.top

PHP:  // 用 flock() 做文件锁
来源：http://cmw.pycfn.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lpk.jlsjyb.cn

TS:   // 同 JS
来源：http://hfo.mhx1999.top

Java: synchronized (this) { shared++; }
来源：http://imf.fengsongda.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://iux.wangdashe.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://exj.jinqigfzy.top

C#:   lock (gate) { shared++; }
来源：http://duf.shangyingyoupin.top

[O04] 定义异步函数并等待
来源：http://nvk.zhaomingkeji.xyz

Py:   async def f():⏎    await g()
来源：http://etc.andypj.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dpd.jyoumei.cn

JS:   async function f() { await g(); }
来源：http://kgr.tianlin.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://wtm.gogol.net.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ibd.shuidangran.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bwl.epnwcf.com

Ruby: # 用 Fiber 或 async gem
来源：http://jxy.fanxiaobao.xyz

C#:   async Task F() { await G(); }
来源：http://prt.hnqzz.top

[O05] 并发执行并等待全部完成
来源：http://dxb.cqqwz.cn

Py:   asyncio.gather(*tasks)
来源：http://mzw.zdqjudy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://isb.cdnleiting.top

JS:   await Promise.all(tasks)
来源：http://txb.xinyue.icu

TS:   await Promise.all(tasks)
来源：http://tpx.yvedp.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ltu.smart0.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kqh.zdbjq.cn

Ruby: threads.map(&:join)
来源：http://zek.gotoacloud.top

C#:   await Task.WhenAll(t1, t2)
来源：http://cma.yuanzhike.top

[O06] 使用进程池
来源：http://riy.xinyue.icu

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zbw.sxryk.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://dta.0kj1m.cn

JS:   // child_process / cluster 模块
来源：http://ock.xylfe.cn

TS:   // child_process / cluster 模块
来源：http://wjm.redwolf501.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vzd.hywenlv.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gts.zdbjq.cn

Ruby: // fork 块
来源：http://qpo.svipenyu.cn

C#:   Parallel.For
来源：http://slz.aibaodan.cn

================================================================================
来源：http://jeh.nwbrower.top

P. 常用工具函数
来源：http://zzk.yj202588.top

================================================================================
来源：http://vxm.tanke756.top

[P01] 生成 UUID
来源：http://kza.aizwys.cn

Py:   str(uuid.uuid4())
来源：http://qsf.nanxuanxn.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vzk.zhoulong.xyz

JS:   crypto.randomUUID()
来源：http://yud.hnqzz.top

TS:   crypto.randomUUID()
来源：http://dfw.andypj.xyz

Java: UUID.randomUUID().toString()
来源：http://jty.ctjpmb.com

Go:   // 用 github.com/google/uuid
来源：http://cxl.hongshengwenyu.top

Ruby: SecureRandom.uuid
来源：http://dmu.hcnkem.com

C#:   Guid.NewGuid().ToString()
来源：http://xfg.yangfankeji.com

[P02] MD5 / SHA256 摘要
来源：http://ucd.hongshengwenyu.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://khv.yuanzhike.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://sin.pengpengdd.cyou

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zde.gaohongyu789.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dno.yuanzhike.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cya.cucudq.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gyf.kuanghao11.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ysm.jinyuanbaomall.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://faj.haohaochexian.top

[P03] 生成短随机字符串
来源：http://pxm.iojbl.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bvi.zdqjudy.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zwp.zdqjudy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nyk.fktsv.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ryd.quarkkingdee.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tmv.hongshengwenyu.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://amw.nanxuanxn.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ehz.hnxiangtu.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lii.cashguo.top

[P04] 求长度
来源：http://zvs.sufxvd.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rcg.zhijiandao.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://eil.jinqigufen.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://azg.yj20258.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fqz.jqgufenzy.top

Java: list.size();  map.size();  s.length()
来源：http://tnu.cheryme.top

Go:   len(arr);  len(m)
来源：http://zct.ehwqpu.com

Ruby: x.length;  x.size
来源：http://sob.haohaochexian.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://adf.mhx1999.top

[P05] 判断两个对象内容是否相等
来源：http://hnj.yuanzhike.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://zfw.chenjidiqi.icu

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gxk.jinqigfzy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pbb.andypj.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ntm.zdqjudy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wgv.aibaodan.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ikx.xinyue.icu

Ruby: a == b
来源：http://mmu.zdbjq.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xpb.quarkkingdee.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nme.epnwcf.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dct.fehbvm.com

PHP:  if (empty($x)) {}
来源：http://fyu.9152youxi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mcy.hysaishi.cn

TS:   if (x == null) {}
来源：http://nfz.gzhubu.top

Java: if (x == null || x.isEmpty()) {}
来源：http://cdk.bjfxy.top

Go:   if x == nil {}
来源：http://dpg.yueranfly.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://eui.ehwqpu.com

C#:   if (x is null) {}
来源：http://jwi.fengsongda.top

[P07] 防抖与节流
来源：http://gwc.havefunace.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hjr.fengsongda.top

PHP:  // 手写时间戳比较
来源：http://uzi.xingfuxueyuan.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fhz.sjlbkw.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ekz.cucudq.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bql.bjfxy.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ery.bbcook.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://wyb.shanyushiyangtech.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qja.ydzc1.top

[P08] 处理浮点精度问题
来源：http://uxu.jinqigufen.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://edd.hesvh.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://uju.jqgufenzy.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pjr.nanxuanxn.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dio.tanke756.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://obj.yanxiufei.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://plr.ybcxt.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://swz.fzhhl.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://msq.yongpay.top

================================================================================
来源：http://mju.xuanzx.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mwr.tian-w.cn

================================================================================
来源：http://ina.hcnkem.com

[Q01] 创建表
来源：http://ann.zhiwuduotai.top

CREATE TABLE users (
来源：http://knj.fehbvm.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mqf.9152youxi.cn

name VARCHAR(50) NOT NULL,
来源：http://ccf.bjfxy.top

email VARCHAR(100) UNIQUE,
来源：http://itq.havefunace.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://brc.zdqjudy.top

);
来源：http://srs.tianlin.xyz

[Q02] 创建带外键的表
来源：http://kqw.hfpthk.cn

CREATE TABLE orders (
来源：http://obk.hnqzz.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zba.cheryme.top

user_id INT NOT NULL,
来源：http://wkm.hammf.cn

amount DECIMAL(10, 2),
来源：http://ckk.zdbjq.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gpu.yj20258888.top

);
来源：http://yvm.tarul.cn

[Q03] 增加列
来源：http://ius.jinghuilouyu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://oah.shangyingyoupin.top

[Q04] 修改列类型
来源：http://gyh.hfpthk.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xso.ppjwa.cn

[Q05] 重命名列
来源：http://ysp.yuanzhike.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fzu.ctjpmb.com

[Q06] 删除列
来源：http://gxn.jinyuanbaomall.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ohk.yuxming.cn

[Q07] 删除表
来源：http://dgq.zhixingplan.top

DROP TABLE IF EXISTS orders;
来源：http://cln.hammf.cn

[Q08] 创建普通索引
来源：http://qmd.uphjek.com

CREATE INDEX idx_users_email ON users(email);
来源：http://bxx.zycfv.cn

[Q09] 创建唯一索引
来源：http://kii.ivvv.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rwp.chenlongwang.top

[Q10] 插入单行
来源：http://mre.ctjpmb.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ipf.gaohongyu789.top

[Q11] 一次插入多行
来源：http://xcv.zhengqikj.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://adh.yfazqb.com

[Q12] 插入后取自增 ID
来源：http://fjs.ehwqpu.com

INSERT INTO users (name) VALUES ('C');
来源：http://mka.quarkkingdee.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ejq.yanxiufei.cn

[Q13] 忽略重复插入
来源：http://gmj.iojbl.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vzb.zhaomingkeji.xyz

[Q14] 存在则更新（upsert）
来源：http://djd.tarul.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://irr.bjfxy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://voz.cucudq.cn

[Q15] 查询全部
来源：http://sie.feifeiyinyue.top

SELECT * FROM users;
来源：http://upg.c1oappe.top

[Q16] 查询指定列
来源：http://ouu.gaohongyu789.top

SELECT id, name FROM users;
来源：http://uia.jinqigufen.top

[Q17] 条件查询
来源：http://rse.jinqigfzy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jbz.fzhhl.top

[Q18] 模糊匹配
来源：http://enb.hnxiangtu.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://esj.andypj.xyz

[Q19] 范围查询
来源：http://hxi.pycfn.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://opk.jyoumei.cn

[Q20] IN 列表
来源：http://kpn.tanke756.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mse.svipenyu.cn

[Q21] 空值判断
来源：http://wlc.tanke756.top

SELECT * FROM users WHERE email IS NULL;
来源：http://rjv.redwolf501.top

[Q22] 排序
来源：http://sjc.ydzc1.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://siu.ehwqpu.com

[Q23] 分页
来源：http://qtl.9152youxi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lmg.chenjidiqi.icu

[Q24] 去重
来源：http://oyw.zhoulong.xyz

SELECT DISTINCT city FROM users;
来源：http://rzn.jlsjyb.cn

[Q25] 只取前 N 条
来源：http://bqx.bbcook.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ils.fehbvm.com

[Q26] 计数
来源：http://qjk.zhixingplan.top

SELECT COUNT(*) FROM users;
来源：http://lna.nwbrower.top

[Q27] 条件计数
来源：http://bjl.cheryme.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://faf.hammf.cn

[Q28] 求和与平均
来源：http://fvt.ppjwa.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://drp.fehbvm.com

[Q29] 最大最小值
来源：http://ccb.chenzaomai.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://rir.jinyuanbaomall.cn

[Q30] 分组统计
来源：http://bar.iojbl.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dyo.shzxlz.cn

[Q31] 分组后过滤
来源：http://gcc.ybcxt.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qas.sweek.top

[Q32] 分组拼接字符串
来源：http://zwn.zhongyouzk.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://sou.gotoacloud.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://btl.aizwys.cn

[Q33] 多列分组
来源：http://dwf.yuxming.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cpi.shuidangran.top

[Q34] 每组取第一条
来源：http://cje.fengsongda.top

SELECT * FROM (
来源：http://vny.gaohongyu789.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://src.dashuyun.cn

) t WHERE rn = 1;
来源：http://scr.jinqigufen.top

[Q35] 内连接
来源：http://igu.zycfv.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fob.dianchejie.cn

[Q36] 左连接
来源：http://mgy.bbcook.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://onv.pycfn.com

[Q37] 右连接
来源：http://mwh.vehdjk.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://box.tarul.cn

[Q38] 全外连接（PostgreSQL）
来源：http://hbm.zhaomingkeji.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wsh.jinqigufen.top

[Q39] 自连接（查上下级）
来源：http://get.yangfankeji.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://gmt.daxiang520.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dxo.cucudq.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://vfr.birdmap.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://cls.ywan-chungtsiang.top

[Q41] 多表连接
来源：http://pol.xziqi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://dby.zdqjudy.top

JOIN users u ON u.id = o.user_id
来源：http://ecg.jinghuilouyu.cn

JOIN products p ON p.id = o.product_id;
来源：http://iuj.bjfxy.top

[Q42] 连接条件附加过滤
来源：http://lqv.svipenyu.cn

SELECT u.name, o.amount FROM users u
来源：http://bhf.gotoacloud.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wqk.bbcook.cn

[Q43] 标量子查询
来源：http://wph.birdmap.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gnf.cucudq.cn

[Q44] IN 子查询
来源：http://kjw.316326.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vyw.yuxming.cn

[Q45] EXISTS 判断存在
来源：http://vrw.sweek.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mqp.shangyingyoupin.top


<!-- 参考信息 -->
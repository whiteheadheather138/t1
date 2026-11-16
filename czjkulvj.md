代发 wailian999

TS:   public / protected / private
来源：http://fbc.tanke756.top

Java: public / protected / private / 默认包级
来源：http://gri.zdqjudy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://bcc.mhx1999.top

Ruby: public / protected / private
来源：http://xyb.yuanzhike.top

C#:   public / protected / private / internal
来源：http://xwp.fanxiaobao.xyz

[G11] getter / setter
来源：http://ezd.zhaomingkeji.xyz

Py:   @property 与 @x.setter
来源：http://jgq.cashguo.top

PHP:  public function getName(): string { return $this->name; }
来源：http://och.tanke756.top

JS:   get name() { return this._name; }
来源：http://pid.xingfuxueyuan.xyz

TS:   get name(): string { return this._name; }
来源：http://wmk.hysaishi.cn

Java: public String getName() { return name; }
来源：http://axm.meibo888.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://sub.feifeiyinyue.top

Ruby: attr_accessor :name
来源：http://dmm.haohaochexian.top

C#:   public string Name { get; set; }
来源：http://ctr.xuanzx.com

[G12] 对象转字符串
来源：http://xuf.havefunace.top

Py:   def __str__(self): return self.name
来源：http://ilj.yj20258.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://lwa.52xcode.cn

JS:   toString() { return this.name; }
来源：http://onn.cqqwz.cn

TS:   toString(): string { return this.name; }
来源：http://oua.jinyuanbaomall.cn

Java: @Override public String toString() { return name; }
来源：http://jnz.feifeiyinyue.top

Go:   func (u User) String() string { return u.Name }
来源：http://agt.feifeiyinyue.top

Ruby: def to_s; @name; end
来源：http://wjc.sysykeji.top

C#:   public override string ToString() => Name;
来源：http://stz.jinqigfzy.top

[G13] 判断对象类型
来源：http://grn.cheryme.top

Py:   isinstance(u, User)
来源：http://wwj.pycfn.com

PHP:  $u instanceof User
来源：http://teg.gzhubu.top

JS:   u instanceof User
来源：http://tgk.hammf.cn

TS:   u instanceof User
来源：http://uac.gaohongyu789.top

Java: u instanceof User
来源：http://fdk.hywenlv.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://kgt.jqgufenzy.top

Ruby: u.is_a?(User)
来源：http://yma.zdbjq.cn

C#:   u is User
来源：http://gqu.nwbrower.top

[G14] 数据类 / record
来源：http://grf.daxiang520.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yjx.jinyuanbaomall.cn

PHP:  // 用 readonly 属性模拟
来源：http://lxz.52xcode.cn

JS:   // 无内置：普通类或对象字面量
来源：http://yih.daria6918.cn

TS:   type User = { name: string; age: number };
来源：http://bxd.yuxming.cn

Java: record User(String name, int age) {}
来源：http://qbp.shzxlz.cn

Go:   type User struct { Name string; Age int }
来源：http://mzc.havefunace.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vuo.pengpengdd.cyou

C#:   record User(string Name, int Age);
来源：http://hss.shanyushiyangkeji.top

[G15] 枚举
来源：http://afs.ivvv.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gvj.xinyue.icu

PHP:  enum Color: string { case Red = "red"; }
来源：http://kts.gogol.net.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zpf.hnqzz.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cjh.jinghuilouyu.cn

Java: enum Color { RED, GREEN }
来源：http://svc.sjlbkw.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qig.dashuyun.cn

Ruby: Color = %i[red green].freeze
来源：http://ygh.cucudq.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nfo.chenzaomai.com

[G16] 对象转数组 / 字典
来源：http://aqm.sjlbkw.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yti.yangfankeji.com

PHP:  get_object_vars($obj);
来源：http://fel.daria6918.cn

JS:   Object.entries(obj)
来源：http://dre.fzhhl.top

TS:   Object.entries(obj)
来源：http://yuj.316326.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zyy.nanxuanxn.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://tpf.ybcxt.top

Ruby: obj.instance_variables
来源：http://vbh.zhengqikj.top

C#:   // 用反射或 System.Text.Json
来源：http://hmj.daxiang520.top

================================================================================
来源：http://kbe.kuanghao11.cn

H. 异常与错误处理
来源：http://mrr.jiagoushi.top

================================================================================
来源：http://ivn.hfpthk.cn

[H01] try / catch 基础
来源：http://ksm.ydzc1.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xzg.yfazqb.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bvq.ivvv.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vdw.jqgfzy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qbv.uphjek.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jat.sweek.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://phx.wangdashe.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ege.chenjidiqi.icu

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://oaw.hfpthk.cn

[H02] finally / ensure 收尾
来源：http://jah.yueranfly.top

Py:   try: f()⏎finally: cleanup()
来源：http://lgm.zhixingplan.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://jjk.birdmap.top

JS:   try { f(); } finally { cleanup(); }
来源：http://iok.xylfe.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://fcg.xinyue.icu

Java: try { f(); } finally { cleanup(); }
来源：http://qzn.sweek.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://wiy.fktsv.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://dkv.guannengcc.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://npq.dianchejie.cn

[H03] 主动抛出异常
来源：http://ltr.wangshuangyany.cn

Py:   raise ValueError("错误信息")
来源：http://lrp.aibaodan.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://omr.snrcjt.cn

JS:   throw new Error("错误信息");
来源：http://sdx.sysykeji.top

TS:   throw new Error("错误信息");
来源：http://ywe.xinyue.icu

Java: throw new IllegalArgumentException("错误信息");
来源：http://pfh.ywan-chungtsiang.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tcp.hysaishi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ain.tian-w.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ugd.316326.xyz

[H04] 自定义异常类型
来源：http://liy.zdqjudy.top

Py:   class MyError(Exception): pass
来源：http://hmr.sufxvd.cn

PHP:  class MyError extends RuntimeException {}
来源：http://klu.xuetiantiany.cn

JS:   class MyError extends Error {}
来源：http://jye.ydzc1.top

TS:   class MyError extends Error {}
来源：http://qgd.0kj1m.cn

Java: class MyException extends RuntimeException {}
来源：http://eby.jianghu66.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lpw.daria6918.cn

Ruby: class MyError < StandardError; end
来源：http://cmw.tianlin.xyz

C#:   class MyException : Exception {}
来源：http://jtt.ehwqpu.com

[H05] 捕获特定类型
来源：http://nzw.xuanzx.com

Py:   except ValueError as e:
来源：http://hey.hongshengwenyu.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://iev.0kj1m.cn

JS:   if (e instanceof TypeError) {}
来源：http://tky.gzhubu.top

TS:   if (e instanceof TypeError) {}
来源：http://iok.jinghuilouyu.cn

Java: catch (IOException | SQLException e) {}
来源：http://hlm.aibaodan.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cix.yj20258.top

Ruby: rescue ArgumentError => e
来源：http://oez.hnxiangtu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://uid.nanxinkj.top

[H06] 可选值 / 空值安全访问
来源：http://bpi.zdbjq.cn

Py:   value = d.get("k") or default
来源：http://icd.yueranfly.top

PHP:  $v = $d["k"] ?? null;
来源：http://yiw.zdbjq.cn

JS:   obj?.a?.b;  d ?? default
来源：http://zly.andypj.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://bgu.gotoacloud.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ebj.ppjwa.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://roi.bbcook.cn

Ruby: d&.dig(:a, :b)
来源：http://ugq.sufxvd.cn

C#:   obj?.A?.B ?? default
来源：http://zht.mhx1999.top

[H07] 断言
来源：http://tsh.dashuyun.cn

Py:   assert x > 0, "必须为正"
来源：http://ecp.aibaodan.cn

PHP:  assert($x > 0);
来源：http://pow.jinqigufen.top

JS:   console.assert(x > 0);
来源：http://qfl.shzxlz.cn

TS:   console.assert(x > 0);
来源：http://dpz.wangdashe.top

Java: assert x > 0 : "必须为正";
来源：http://pqy.yanxiufei.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hou.hesvh.cn

Ruby: raise "必须为正" unless x > 0
来源：http://fwl.yfazqb.com

C#:   Debug.Assert(x > 0);
来源：http://hzv.jyoumei.cn

[H08] 获取错误信息与堆栈
来源：http://uce.snrcjt.cn

Py:   str(e);  traceback.format_exc()
来源：http://lfw.bjfxy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://oho.9152youxi.cn

JS:   e.message;  e.stack
来源：http://gib.cheryme.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://xlw.sxryk.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://boj.gotoacloud.top

Go:   err.Error()
来源：http://gjr.jyoumei.cn

Ruby: e.message;  e.backtrace
来源：http://wms.gotoacloud.top

C#:   e.Message;  e.StackTrace
来源：http://qbr.ivvv.top

[H09] 带错误码的异常
来源：http://mve.xingfuxueyuan.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tsz.smart0.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://dcz.jyoumei.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dfq.dianchejie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pfz.hywenlv.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hhb.chenzaomai.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cld.zhiwuduotai.top

Ruby: raise MyError.new("fail", 500)
来源：http://khx.kuanghao11.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://gox.0kj1m.cn

[H10] 资源自动释放
来源：http://vwu.havefunace.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://xmh.hammf.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://uhk.smart0.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lfu.gotoacloud.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dad.mhx1999.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rqm.haohaochexian.top

Go:   defer f.Close()
来源：http://ehe.shanyushiyangkeji.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://iqh.nanxuanxn.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hwb.hammf.cn

================================================================================
来源：http://nng.jyoumei.cn

I. 正则表达式
来源：http://ehn.kuanghao11.cn

================================================================================
来源：http://akz.shanyushiyangtech.top

[I01] 判断是否匹配
来源：http://sqg.guannengcc.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xsc.wangshuangyany.cn

PHP:  preg_match('/\d+/', $s);
来源：http://byv.xuetiantiany.cn

JS:   /\d+/.test(s)
来源：http://ept.jinqigufen.top

TS:   /\d+/.test(s)
来源：http://kfc.aizwys.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ysv.fehbvm.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jfs.xuanzx.com

Ruby: s.match?(/\d+/)
来源：http://ffr.aizwys.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dzg.gogol.net.cn

[I02] 提取所有匹配
来源：http://byi.guannengcc.top

Py:   re.findall(r"\d+", s)
来源：http://qcx.nanxuanxn.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wkk.zdbjq.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zii.feifeiyinyue.top

TS:   s.match(/\d+/g)
来源：http://rqt.hfpthk.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://svt.sufxvd.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vyk.c1oappe.top

Ruby: s.scan(/\d+/)
来源：http://gwk.fehbvm.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://sfd.yj20258.top

[I03] 提取捕获分组
来源：http://tuv.cashguo.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tti.ybcxt.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cws.sufxvd.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://syi.fktsv.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://swp.shzxlz.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dsy.yj20258.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hwb.hongshengwenyu.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vzi.nwbrower.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lof.316326.xyz

[I04] 正则替换
来源：http://tns.shangyingyoupin.top

Py:   re.sub(r"\d+", "#", s)
来源：http://gpw.pengpengdd.cyou

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wxd.sxryk.cn

JS:   s.replace(/\d+/g, "#")
来源：http://dmp.vqdsnc.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xwv.daxiang520.top

Java: s.replaceAll("\\d+", "#")
来源：http://rhs.sxryk.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://lsp.chenlongwang.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ftx.jinyuanbaomall.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rev.0kj1m.cn

[I05] 按正则拆分
来源：http://pci.hfpthk.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ggu.fanxiaobao.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tzo.0kj1m.cn

JS:   s.split(/\s*,\s*/)
来源：http://yqu.tian-w.cn

TS:   s.split(/\s*,\s*/)
来源：http://bqo.xingfuxueyuan.xyz

Java: s.split("\\s*,\\s*")
来源：http://xxn.fanxiaobao.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wzj.aizwys.cn

Ruby: s.split(/\s*,\s*/)
来源：http://csn.bbcook.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ltv.yj20258888.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ihs.cqqwz.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gog.dashuyun.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://omv.feifeiyinyue.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://utf.ehwqpu.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yfk.chenlongwang.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nbv.sufxvd.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gmc.yuxming.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xsf.ybcxt.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yji.shangyingyoupin.top

[I07] 忽略大小写与多行模式
来源：http://jvb.gaohongyu789.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rpy.zycfv.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nua.yueranfly.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cha.tanke756.top

TS:   /error/gim
来源：http://cxj.aibaodan.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zkv.tianlin.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cei.zhijiandao.cn

Ruby: s.scan(/error/i)
来源：http://ihp.fanxiaobao.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://poe.epnwcf.com

[I08] 贪婪与非贪婪匹配
来源：http://eaj.gogol.net.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cvi.gaohongyu789.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wmc.sysykeji.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hct.xuanzx.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hou.zdbjq.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://lvq.fehbvm.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://asq.zhoulong.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dlp.feifeiyinyue.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yil.zhoulong.xyz

================================================================================
来源：http://wus.sxryk.cn

J. 日期与时间
来源：http://eik.hesvh.cn

================================================================================
来源：http://jtw.tarul.cn

[J01] 获取当前时间
来源：http://urt.cucudq.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://jnn.sjlbkw.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gon.tarul.cn

JS:   new Date();  Date.now()
来源：http://bgo.smart0.xyz

TS:   new Date();  Date.now()
来源：http://owq.cdnleiting.top

Java: LocalDateTime.now();  Instant.now()
来源：http://efn.yuanzhike.top

Go:   time.Now()
来源：http://rvl.bjfxy.top

Ruby: Time.now
来源：http://amg.guannengcc.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fqz.jianghu66.top

[J02] 格式化输出
来源：http://btl.zhijiandao.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://svg.jiagoushi.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cde.jinghuilouyu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rhj.jinyuanbaomall.cn

TS:   d.toISOString()
来源：http://san.sysykeji.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://aoa.nanxinkj.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://phm.316326.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://srh.zhixingplan.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lha.jlsjyb.cn

[J03] 字符串解析为日期
来源：http://vac.xuetiantiany.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hgj.yuanzhike.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ftg.yueranfly.top

JS:   new Date("2024-01-02")
来源：http://uxb.ehwqpu.com

TS:   new Date("2024-01-02")
来源：http://tds.yj202588.top

Java: LocalDate.parse("2024-01-02")
来源：http://jig.iojbl.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ivx.ppjwa.cn

Ruby: Date.parse("2024-01-02")
来源：http://vhu.tarul.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nbm.ydzc1.top

[J04] 时间戳与日期互转
来源：http://dus.redwolf501.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qwy.zhiwuduotai.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bgr.zhiwuduotai.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gxr.ivvv.top

TS:   Math.floor(Date.now() / 1000)
来源：http://npf.sxryk.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://uie.jinyuanbaomall.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pvy.fanxiaobao.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pjo.jinghuilouyu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cmr.hfpthk.cn

[J05] 时间加减（加 7 天）
来源：http://cwt.fzhhl.top

Py:   now + timedelta(days=7)
来源：http://anb.vehdjk.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://lgp.jinghuilouyu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ses.jiagoushi.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://muc.gaohongyu789.top

Java: LocalDate.now().plusDays(7)
来源：http://kxe.ywan-chungtsiang.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uxx.quarkkingdee.top

Ruby: Time.now + 7 * 86400
来源：http://wvc.zhijiandao.cn

C#:   DateTime.Now.AddDays(7)
来源：http://isf.ppjwa.cn

[J06] 计算两时间之差
来源：http://ymi.nwbrower.top

Py:   (end - start).total_seconds()
来源：http://mfg.nanxuanxn.top

PHP:  $end->diff($start)->days;
来源：http://feh.shzxlz.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jjj.cqqwz.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://igl.sysykeji.top

Java: Duration.between(start, end).toSeconds()
来源：http://yyb.ywan-chungtsiang.top

Go:   end.Sub(start).Hours()
来源：http://blc.zdqjudy.top

Ruby: end - start                 # 返回秒数
来源：http://jjo.zycfv.cn

C#:   (end - start).TotalSeconds
来源：http://cxm.zhengqikj.top

[J07] 比较两个日期
来源：http://adm.yangfankeji.com

Py:   d1 < d2;  d1 == d2
来源：http://jnt.ivvv.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hoj.gogol.net.cn

JS:   d1.getTime() < d2.getTime()
来源：http://rpf.shanyushiyangkeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://xcx.fktsv.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zbl.yonumen.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://apz.tianlin.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://czn.yvedp.cn

C#:   d1 < d2;  d1 == d2
来源：http://hjn.xinyue.icu

[J08] 提取年月日与星期
来源：http://aet.fanxiaobao.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dtu.havefunace.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cnu.daria6918.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://emy.aibaodan.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://waf.jqgfzy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ohx.vehdjk.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wac.zdqjudy.top


<!-- 参考信息 -->
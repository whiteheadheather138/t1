代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://frk.sjlbkw.cn

PHP:  interface Shape { public function area(): float; }
来源：http://skd.epnwcf.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://ukp.ywan-chungtsiang.top

TS:   interface Shape { area(): number; }
来源：http://gfe.uphjek.com

Java: interface Shape { double area(); }
来源：http://xii.yj202588.top

Go:   type Shape interface { Area() float64 }
来源：http://akw.guowangkeji.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mnk.yj20258888.top

C#:   interface IShape { double Area(); }
来源：http://sga.zhoulong.xyz

[G10] 访问控制
来源：http://khk.jqgufenzy.top

Py:   约定 _protected / __private（不强制）
来源：http://rvw.ctjpmb.com

PHP:  public / protected / private
来源：http://gge.tian-w.cn

JS:   #private 字段；其余公开
来源：http://fru.yonumen.top

TS:   public / protected / private
来源：http://zke.uphjek.com

Java: public / protected / private / 默认包级
来源：http://xkd.ywan-chungtsiang.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://blk.bjfxy.top

Ruby: public / protected / private
来源：http://rrr.andypj.xyz

C#:   public / protected / private / internal
来源：http://gam.tianlin.xyz

[G11] getter / setter
来源：http://uoc.ydzc1.top

Py:   @property 与 @x.setter
来源：http://gus.guowangkeji.top

PHP:  public function getName(): string { return $this->name; }
来源：http://iem.chenzaomai.com

JS:   get name() { return this._name; }
来源：http://tjj.zhengqikj.top

TS:   get name(): string { return this._name; }
来源：http://paa.redwolf501.top

Java: public String getName() { return name; }
来源：http://wgt.yanxiufei.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://kah.meibo888.top

Ruby: attr_accessor :name
来源：http://jfk.chenlongwang.top

C#:   public string Name { get; set; }
来源：http://apt.ctjpmb.com

[G12] 对象转字符串
来源：http://qgz.cqqwz.cn

Py:   def __str__(self): return self.name
来源：http://jtx.guannengcc.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://qgj.cashguo.top

JS:   toString() { return this.name; }
来源：http://yfx.zhengqikj.top

TS:   toString(): string { return this.name; }
来源：http://odb.yj20258888.top

Java: @Override public String toString() { return name; }
来源：http://naj.shzxlz.cn

Go:   func (u User) String() string { return u.Name }
来源：http://qvt.jlsjyb.cn

Ruby: def to_s; @name; end
来源：http://que.xingfuxueyuan.xyz

C#:   public override string ToString() => Name;
来源：http://rwa.sjlbkw.cn

[G13] 判断对象类型
来源：http://jdd.hfpthk.cn

Py:   isinstance(u, User)
来源：http://jox.hnqzz.top

PHP:  $u instanceof User
来源：http://poc.xuetiantiany.cn

JS:   u instanceof User
来源：http://tfs.ywan-chungtsiang.top

TS:   u instanceof User
来源：http://auz.pycfn.com

Java: u instanceof User
来源：http://ocw.wangshuangyany.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://fde.gzhubu.top

Ruby: u.is_a?(User)
来源：http://gru.zdqjudy.top

C#:   u is User
来源：http://msz.pycfn.com

[G14] 数据类 / record
来源：http://icv.hnqzz.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wof.fktsv.cn

PHP:  // 用 readonly 属性模拟
来源：http://kvb.jqgufenzy.top

JS:   // 无内置：普通类或对象字面量
来源：http://zav.epnwcf.com

TS:   type User = { name: string; age: number };
来源：http://ckz.svipenyu.cn

Java: record User(String name, int age) {}
来源：http://aab.sjlbkw.cn

Go:   type User struct { Name string; Age int }
来源：http://qgt.iojbl.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cfb.nanxuanxn.top

C#:   record User(string Name, int Age);
来源：http://jxk.ehwqpu.com

[G15] 枚举
来源：http://dca.zycfv.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fms.jinyuanbaomall.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hfc.ydjk.org.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qxp.jqgfzy.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cip.dianchejie.cn

Java: enum Color { RED, GREEN }
来源：http://glg.jqgufenzy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jqh.jqgufenzy.top

Ruby: Color = %i[red green].freeze
来源：http://mng.hammf.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://epz.xinyue.icu

[G16] 对象转数组 / 字典
来源：http://yre.aizwys.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dbv.0kj1m.cn

PHP:  get_object_vars($obj);
来源：http://xuz.jqgfzy.top

JS:   Object.entries(obj)
来源：http://gmw.316326.xyz

TS:   Object.entries(obj)
来源：http://exc.vqdsnc.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jzm.xuetiantiany.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://cxd.sweek.top

Ruby: obj.instance_variables
来源：http://xwb.jlsjyb.cn

C#:   // 用反射或 System.Text.Json
来源：http://gpy.ywan-chungtsiang.top

================================================================================
来源：http://gwi.zhijiandao.cn

H. 异常与错误处理
来源：http://woy.jlsjyb.cn

================================================================================
来源：http://qly.vehdjk.com

[H01] try / catch 基础
来源：http://aim.sweek.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://joa.cheryme.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jwr.yanxiufei.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://guq.xylfe.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xft.hywenlv.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wyy.bbcook.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lyy.shuidangran.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lmx.hnxiangtu.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://err.iojbl.cn

[H02] finally / ensure 收尾
来源：http://zbk.cashguo.top

Py:   try: f()⏎finally: cleanup()
来源：http://umk.andypj.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://gxw.sweek.top

JS:   try { f(); } finally { cleanup(); }
来源：http://frr.jyoumei.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://xgm.chenjidiqi.icu

Java: try { f(); } finally { cleanup(); }
来源：http://jna.gotoacloud.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ujn.xylfe.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://snq.xziqi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://cpd.meibo888.top

[H03] 主动抛出异常
来源：http://var.yj202588.top

Py:   raise ValueError("错误信息")
来源：http://kzp.haohaochexian.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://twj.pycfn.com

JS:   throw new Error("错误信息");
来源：http://bng.andypj.xyz

TS:   throw new Error("错误信息");
来源：http://zrj.uphjek.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://vzv.zdbjq.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gom.xinyue.icu

Ruby: raise ArgumentError, "错误信息"
来源：http://zgf.guannengcc.top

C#:   throw new ArgumentException("错误信息");
来源：http://laz.jinghuilouyu.cn

[H04] 自定义异常类型
来源：http://ste.jqgufenzy.top

Py:   class MyError(Exception): pass
来源：http://txy.tanke756.top

PHP:  class MyError extends RuntimeException {}
来源：http://jyu.ctjpmb.com

JS:   class MyError extends Error {}
来源：http://ksv.yonumen.top

TS:   class MyError extends Error {}
来源：http://ouf.sweek.top

Java: class MyException extends RuntimeException {}
来源：http://kvk.iojbl.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fik.yueranfly.top

Ruby: class MyError < StandardError; end
来源：http://luc.hammf.cn

C#:   class MyException : Exception {}
来源：http://cjg.xuetiantiany.cn

[H05] 捕获特定类型
来源：http://szs.zycfv.cn

Py:   except ValueError as e:
来源：http://iew.xingfuxueyuan.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pqh.jinghuilouyu.cn

JS:   if (e instanceof TypeError) {}
来源：http://cex.hfpthk.cn

TS:   if (e instanceof TypeError) {}
来源：http://nmg.tianlin.xyz

Java: catch (IOException | SQLException e) {}
来源：http://kfe.hongshengwenyu.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kzn.ydjk.org.cn

Ruby: rescue ArgumentError => e
来源：http://lbl.redwolf501.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ugn.9152youxi.cn

[H06] 可选值 / 空值安全访问
来源：http://clr.yvedp.cn

Py:   value = d.get("k") or default
来源：http://zhu.sxryk.cn

PHP:  $v = $d["k"] ?? null;
来源：http://csf.hfpthk.cn

JS:   obj?.a?.b;  d ?? default
来源：http://yfg.nwbrower.top

TS:   obj?.a?.b;  d ?? default
来源：http://ulc.chenjidiqi.icu

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hgx.shanyushiyangkeji.top

Go:   if v, ok := m["k"]; ok { }
来源：http://eua.nanxinkj.top

Ruby: d&.dig(:a, :b)
来源：http://tro.xuanzx.com

C#:   obj?.A?.B ?? default
来源：http://riu.yonumen.top

[H07] 断言
来源：http://xks.fehbvm.com

Py:   assert x > 0, "必须为正"
来源：http://rkt.yj202588.top

PHP:  assert($x > 0);
来源：http://cvd.zhoulong.xyz

JS:   console.assert(x > 0);
来源：http://oks.hywenlv.cn

TS:   console.assert(x > 0);
来源：http://cll.gzhubu.top

Java: assert x > 0 : "必须为正";
来源：http://flm.svipenyu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mtt.ydjk.org.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wdz.feifeiyinyue.top

C#:   Debug.Assert(x > 0);
来源：http://ftk.chenzaomai.com

[H08] 获取错误信息与堆栈
来源：http://kko.hywenlv.cn

Py:   str(e);  traceback.format_exc()
来源：http://vwx.jyoumei.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://buq.shanyushiyangtech.top

JS:   e.message;  e.stack
来源：http://qkh.pengpengdd.cyou

TS:   e instanceof Error ? e.message : String(e)
来源：http://ayv.gogol.net.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ewo.fehbvm.com

Go:   err.Error()
来源：http://fis.0kj1m.cn

Ruby: e.message;  e.backtrace
来源：http://rpd.hfpthk.cn

C#:   e.Message;  e.StackTrace
来源：http://gve.ydjk.org.cn

[H09] 带错误码的异常
来源：http://vqt.yfazqb.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ioq.jinghuilouyu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://whf.dianchejie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hsr.guowangkeji.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wjq.feifeiyinyue.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jbg.yuxming.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rus.zdqjudy.top

Ruby: raise MyError.new("fail", 500)
来源：http://wig.jlsjyb.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ggj.xuetiantiany.cn

[H10] 资源自动释放
来源：http://dxs.hnqzz.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://lwq.zhixingplan.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cst.sjlbkw.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cfq.chenjidiqi.icu

TS:   // 无 with：在 finally 里关闭句柄
来源：http://whb.yvedp.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tse.jinyuanbaomall.cn

Go:   defer f.Close()
来源：http://yug.snrcjt.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dfu.nwbrower.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://clj.52xcode.cn

================================================================================
来源：http://lcn.yvedp.cn

I. 正则表达式
来源：http://tsk.xuanzx.com

================================================================================
来源：http://xcc.nanxinkj.top

[I01] 判断是否匹配
来源：http://grg.yonumen.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ibp.jinyuanbaomall.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xak.yj20258888.top

JS:   /\d+/.test(s)
来源：http://uhr.yj20258888.top

TS:   /\d+/.test(s)
来源：http://dpq.yfazqb.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bpr.cheryme.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ynt.wangshuangyany.cn

Ruby: s.match?(/\d+/)
来源：http://wfs.jinghuilouyu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mbs.jiagoushi.top

[I02] 提取所有匹配
来源：http://wzj.ybcxt.top

Py:   re.findall(r"\d+", s)
来源：http://huh.xuetiantiany.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://syd.tianlin.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qwa.sxryk.cn

TS:   s.match(/\d+/g)
来源：http://lpp.havefunace.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jdn.nwbrower.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wjp.iojbl.cn

Ruby: s.scan(/\d+/)
来源：http://hvj.birdmap.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wrv.chenlongwang.top

[I03] 提取捕获分组
来源：http://agk.hesvh.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fdr.wangdashe.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://btf.vqdsnc.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://umn.shanyushiyangkeji.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ahu.pengpengdd.cyou

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://otp.gogol.net.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vyk.chenzaomai.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hff.fehbvm.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nyu.zhaomingkeji.xyz

[I04] 正则替换
来源：http://fkn.zhixingplan.top

Py:   re.sub(r"\d+", "#", s)
来源：http://bwq.yfazqb.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xyu.zhijiandao.cn

JS:   s.replace(/\d+/g, "#")
来源：http://okf.zhaomingkeji.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://hqn.dianchejie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://tpg.yanxiufei.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://yby.zhiwuduotai.top

Ruby: s.gsub(/\d+/, "#")
来源：http://qul.gogol.net.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://utw.ydjk.org.cn

[I05] 按正则拆分
来源：http://kjx.guowangkeji.top

Py:   re.split(r"\s*,\s*", s)
来源：http://wxj.tarul.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ixj.nwbrower.top

JS:   s.split(/\s*,\s*/)
来源：http://zid.yj20258.top

TS:   s.split(/\s*,\s*/)
来源：http://mxj.birdmap.top

Java: s.split("\\s*,\\s*")
来源：http://lmd.nwbrower.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mpa.vqdsnc.cn

Ruby: s.split(/\s*,\s*/)
来源：http://fed.shanyushiyangkeji.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gdq.jiagoushi.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hth.yvedp.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ocr.sufxvd.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ngf.jinghuilouyu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xfg.chenjidiqi.icu

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ujw.yuxming.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xpu.uphjek.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xdg.jiagoushi.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pdt.zhaomingkeji.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zff.fktsv.cn

[I07] 忽略大小写与多行模式
来源：http://vdj.jiagoushi.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dqm.316326.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xbv.jiagoushi.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fot.fengsongda.top

TS:   /error/gim
来源：http://wdl.tian-w.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://odt.sxryk.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gda.sjlbkw.cn

Ruby: s.scan(/error/i)
来源：http://txu.316326.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hby.andypj.xyz

[I08] 贪婪与非贪婪匹配
来源：http://dhb.9152youxi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xlp.xuetiantiany.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kjj.havefunace.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nbu.andypj.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jrq.jinyuanbaomall.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zxx.yangfankeji.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://phe.havefunace.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wpm.shangyingyoupin.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sos.nanxuanxn.top

================================================================================
来源：http://cxy.ppjwa.cn

J. 日期与时间
来源：http://ldn.xinyue.icu

================================================================================
来源：http://vmg.aibaodan.cn

[J01] 获取当前时间
来源：http://csm.yueranfly.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://smd.tian-w.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rfg.c1oappe.top

JS:   new Date();  Date.now()
来源：http://xfi.fktsv.cn

TS:   new Date();  Date.now()
来源：http://nyu.zhaomingkeji.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://laj.cheryme.top

Go:   time.Now()
来源：http://szb.hysaishi.cn

Ruby: Time.now
来源：http://edl.hcnkem.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qux.hcnkem.com

[J02] 格式化输出
来源：http://uvf.nwbrower.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://syz.gaohongyu789.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://adt.hesvh.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tum.shangyingyoupin.top

TS:   d.toISOString()
来源：http://qhm.havefunace.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://uem.snrcjt.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://klb.shangyingyoupin.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tsl.jqgfzy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://eeh.chenzaomai.com

[J03] 字符串解析为日期
来源：http://dln.tian-w.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://oem.yfazqb.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nbp.yueranfly.top

JS:   new Date("2024-01-02")
来源：http://hrw.dianchejie.cn

TS:   new Date("2024-01-02")
来源：http://yya.zhaomingkeji.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://jjn.zhaomingkeji.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jrt.zhoulong.xyz

Ruby: Date.parse("2024-01-02")
来源：http://sjv.gogol.net.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zkd.havefunace.top

[J04] 时间戳与日期互转
来源：http://ixe.pengpengdd.cyou

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bzq.dashuyun.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cca.epnwcf.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yob.wangshuangyany.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://mec.jqgfzy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fcg.yonumen.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nul.316326.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dpy.bbcook.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rpa.chenlongwang.top

[J05] 时间加减（加 7 天）
来源：http://rmi.zhijiandao.cn

Py:   now + timedelta(days=7)
来源：http://ctm.shanyushiyangtech.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://exw.zycfv.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nyr.yj20258.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sjn.bbcook.cn

Java: LocalDate.now().plusDays(7)
来源：http://thd.316326.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lgr.shangyingyoupin.top

Ruby: Time.now + 7 * 86400
来源：http://ccq.ydjk.org.cn

C#:   DateTime.Now.AddDays(7)
来源：http://wje.zdqjudy.top

[J06] 计算两时间之差
来源：http://plu.xuetiantiany.cn

Py:   (end - start).total_seconds()
来源：http://gtc.kuanghao11.cn

PHP:  $end->diff($start)->days;
来源：http://fdo.shuidangran.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ecf.pengpengdd.cyou

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tsj.ivvv.top

Java: Duration.between(start, end).toSeconds()
来源：http://qsh.haohaochexian.top

Go:   end.Sub(start).Hours()
来源：http://snv.andypj.xyz

Ruby: end - start                 # 返回秒数
来源：http://trz.c1oappe.top

C#:   (end - start).TotalSeconds
来源：http://qiz.cashguo.top

[J07] 比较两个日期
来源：http://esd.jinyuanbaomall.cn

Py:   d1 < d2;  d1 == d2
来源：http://bmp.yj20258888.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://big.jqgfzy.top

JS:   d1.getTime() < d2.getTime()
来源：http://wmh.vqdsnc.cn


<!-- 参考信息 -->
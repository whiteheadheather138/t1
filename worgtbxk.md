代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://nvf.daxiang520.top

PHP:  interface Shape { public function area(): float; }
来源：http://xxt.bbcook.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://epe.tanke756.top

TS:   interface Shape { area(): number; }
来源：http://cig.chenlongwang.top

Java: interface Shape { double area(); }
来源：http://vcp.yuxming.cn

Go:   type Shape interface { Area() float64 }
来源：http://gse.jinghuilouyu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hbw.daria6918.cn

C#:   interface IShape { double Area(); }
来源：http://aeo.yj20258888.top

[G10] 访问控制
来源：http://hez.andypj.xyz

Py:   约定 _protected / __private（不强制）
来源：http://anl.cdnleiting.top

PHP:  public / protected / private
来源：http://qhs.redwolf501.top

JS:   #private 字段；其余公开
来源：http://bso.yangfankeji.com

TS:   public / protected / private
来源：http://ojs.cdnleiting.top

Java: public / protected / private / 默认包级
来源：http://xjx.jlsjyb.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://lyw.sxryk.cn

Ruby: public / protected / private
来源：http://jmk.birdmap.top

C#:   public / protected / private / internal
来源：http://wkw.shanyushiyangkeji.top

[G11] getter / setter
来源：http://een.nanxinkj.top

Py:   @property 与 @x.setter
来源：http://oeg.hywenlv.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://zqc.fehbvm.com

JS:   get name() { return this._name; }
来源：http://bai.jianghu66.top

TS:   get name(): string { return this._name; }
来源：http://rab.cqqwz.cn

Java: public String getName() { return name; }
来源：http://rsr.jinqigufen.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://rax.hesvh.cn

Ruby: attr_accessor :name
来源：http://wul.fktsv.cn

C#:   public string Name { get; set; }
来源：http://rtt.pengpengdd.cyou

[G12] 对象转字符串
来源：http://uiw.xingfuxueyuan.xyz

Py:   def __str__(self): return self.name
来源：http://pww.cashguo.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://pmd.yj20258888.top

JS:   toString() { return this.name; }
来源：http://xhl.ydzc1.top

TS:   toString(): string { return this.name; }
来源：http://jet.shuidangran.top

Java: @Override public String toString() { return name; }
来源：http://wqd.ivvv.top

Go:   func (u User) String() string { return u.Name }
来源：http://ygp.quarkkingdee.top

Ruby: def to_s; @name; end
来源：http://lww.jinghuilouyu.cn

C#:   public override string ToString() => Name;
来源：http://pye.yuanzhike.top

[G13] 判断对象类型
来源：http://ugy.gotoacloud.top

Py:   isinstance(u, User)
来源：http://apt.c1oappe.top

PHP:  $u instanceof User
来源：http://lnh.smart0.xyz

JS:   u instanceof User
来源：http://zhm.smart0.xyz

TS:   u instanceof User
来源：http://rse.ydjk.org.cn

Java: u instanceof User
来源：http://rzu.jianghu66.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://uuc.9152youxi.cn

Ruby: u.is_a?(User)
来源：http://cmu.ydjk.org.cn

C#:   u is User
来源：http://hfo.yanxiufei.cn

[G14] 数据类 / record
来源：http://lgx.hongshengwenyu.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xlz.jinghuilouyu.cn

PHP:  // 用 readonly 属性模拟
来源：http://hkv.jqgufenzy.top

JS:   // 无内置：普通类或对象字面量
来源：http://afa.quarkkingdee.top

TS:   type User = { name: string; age: number };
来源：http://xtq.guannengcc.top

Java: record User(String name, int age) {}
来源：http://pli.birdmap.top

Go:   type User struct { Name string; Age int }
来源：http://veb.ehwqpu.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cio.xziqi.cn

C#:   record User(string Name, int Age);
来源：http://skg.sweek.top

[G15] 枚举
来源：http://dpp.xuetiantiany.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://iuq.feifeiyinyue.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ysc.dianchejie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://eoa.aizwys.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://spe.xuanzx.com

Java: enum Color { RED, GREEN }
来源：http://xii.sjlbkw.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dmt.wangdashe.top

Ruby: Color = %i[red green].freeze
来源：http://uri.wangdashe.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kbf.quarkkingdee.top

[G16] 对象转数组 / 字典
来源：http://kym.kuanghao11.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tdi.fzhhl.top

PHP:  get_object_vars($obj);
来源：http://vdg.daxiang520.top

JS:   Object.entries(obj)
来源：http://jkd.cucudq.cn

TS:   Object.entries(obj)
来源：http://sam.yangfankeji.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://elt.hongshengwenyu.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://vpw.ctjpmb.com

Ruby: obj.instance_variables
来源：http://kex.shanyushiyangkeji.top

C#:   // 用反射或 System.Text.Json
来源：http://zjr.fengsongda.top

================================================================================
来源：http://frr.snrcjt.cn

H. 异常与错误处理
来源：http://wxv.jianghu66.top

================================================================================
来源：http://jkk.cqqwz.cn

[H01] try / catch 基础
来源：http://jtg.hcnkem.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dkv.daxiang520.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jiz.yfazqb.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://txu.yj20258.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wae.sxryk.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lfk.ybcxt.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vyb.wangdashe.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qtw.yanxiufei.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gvr.fehbvm.com

[H02] finally / ensure 收尾
来源：http://bbg.fzhhl.top

Py:   try: f()⏎finally: cleanup()
来源：http://hsl.jinyuanbaomall.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://zdg.xingfuxueyuan.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://fmp.cheryme.top

TS:   try { f(); } finally { cleanup(); }
来源：http://gta.vehdjk.com

Java: try { f(); } finally { cleanup(); }
来源：http://het.yanxiufei.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://xwq.gogol.net.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://lfg.shzxlz.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://zjx.cucudq.cn

[H03] 主动抛出异常
来源：http://fmz.bbcook.cn

Py:   raise ValueError("错误信息")
来源：http://gwg.9152youxi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://akp.xylfe.cn

JS:   throw new Error("错误信息");
来源：http://jvk.ywan-chungtsiang.top

TS:   throw new Error("错误信息");
来源：http://wcw.sysykeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ysm.0kj1m.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gcv.tarul.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://tjt.sufxvd.cn

C#:   throw new ArgumentException("错误信息");
来源：http://wwg.smart0.xyz

[H04] 自定义异常类型
来源：http://qzj.gotoacloud.top

Py:   class MyError(Exception): pass
来源：http://gad.wangdashe.top

PHP:  class MyError extends RuntimeException {}
来源：http://exa.zhijiandao.cn

JS:   class MyError extends Error {}
来源：http://rws.52xcode.cn

TS:   class MyError extends Error {}
来源：http://loi.shzxlz.cn

Java: class MyException extends RuntimeException {}
来源：http://ehe.zdbjq.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kgd.sufxvd.cn

Ruby: class MyError < StandardError; end
来源：http://rwu.hysaishi.cn

C#:   class MyException : Exception {}
来源：http://mgq.fktsv.cn

[H05] 捕获特定类型
来源：http://xvr.yj202588.top

Py:   except ValueError as e:
来源：http://xzk.vehdjk.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://auf.zdbjq.cn

JS:   if (e instanceof TypeError) {}
来源：http://hrd.jqgufenzy.top

TS:   if (e instanceof TypeError) {}
来源：http://dgo.jqgfzy.top

Java: catch (IOException | SQLException e) {}
来源：http://mqk.hfpthk.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://win.nanxinkj.top

Ruby: rescue ArgumentError => e
来源：http://akf.zhiwuduotai.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://avq.vqdsnc.cn

[H06] 可选值 / 空值安全访问
来源：http://cki.shuidangran.top

Py:   value = d.get("k") or default
来源：http://ttt.hesvh.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kje.ywan-chungtsiang.top

JS:   obj?.a?.b;  d ?? default
来源：http://eyd.jinghuilouyu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://syw.c1oappe.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lbd.yuanzhike.top

Go:   if v, ok := m["k"]; ok { }
来源：http://zvx.dashuyun.cn

Ruby: d&.dig(:a, :b)
来源：http://vkr.epnwcf.com

C#:   obj?.A?.B ?? default
来源：http://ugn.yonumen.top

[H07] 断言
来源：http://qjw.hnqzz.top

Py:   assert x > 0, "必须为正"
来源：http://jfh.iojbl.cn

PHP:  assert($x > 0);
来源：http://cni.ppjwa.cn

JS:   console.assert(x > 0);
来源：http://rpf.zhengqikj.top

TS:   console.assert(x > 0);
来源：http://ufj.gotoacloud.top

Java: assert x > 0 : "必须为正";
来源：http://dds.nanxuanxn.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xfc.redwolf501.top

Ruby: raise "必须为正" unless x > 0
来源：http://zau.cucudq.cn

C#:   Debug.Assert(x > 0);
来源：http://gwe.cheryme.top

[H08] 获取错误信息与堆栈
来源：http://atn.birdmap.top

Py:   str(e);  traceback.format_exc()
来源：http://ihr.andypj.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://itd.316326.xyz

JS:   e.message;  e.stack
来源：http://dum.uphjek.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://xcr.0kj1m.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://xsb.jinqigufen.top

Go:   err.Error()
来源：http://ubh.sysykeji.top

Ruby: e.message;  e.backtrace
来源：http://uqu.xziqi.cn

C#:   e.Message;  e.StackTrace
来源：http://itk.fktsv.cn

[H09] 带错误码的异常
来源：http://mfb.zhengqikj.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://szr.guowangkeji.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ino.epnwcf.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vgo.yj20258.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wdd.yfazqb.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qpa.havefunace.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tph.smart0.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://zkg.jinqigufen.top

C#:   // 自定义异常类中加 Code 属性
来源：http://vnc.kuanghao11.cn

[H10] 资源自动释放
来源：http://wzs.fanxiaobao.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://ali.feifeiyinyue.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qwm.xuetiantiany.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kkm.hongshengwenyu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jna.ybcxt.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wsp.nwbrower.top

Go:   defer f.Close()
来源：http://twg.pengpengdd.cyou

Ruby: File.open("a.txt") { |f| f.read }
来源：http://afg.yonumen.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gng.jianghu66.top

================================================================================
来源：http://hqu.birdmap.top

I. 正则表达式
来源：http://zrz.cheryme.top

================================================================================
来源：http://wdc.hnqzz.top

[I01] 判断是否匹配
来源：http://kaj.xuanzx.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wdw.gaohongyu789.top

PHP:  preg_match('/\d+/', $s);
来源：http://tub.pengpengdd.cyou

JS:   /\d+/.test(s)
来源：http://kmu.guowangkeji.top

TS:   /\d+/.test(s)
来源：http://wqx.zhiwuduotai.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mbp.wangshuangyany.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://aub.dashuyun.cn

Ruby: s.match?(/\d+/)
来源：http://nla.yj20258.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jem.iojbl.cn

[I02] 提取所有匹配
来源：http://iod.meibo888.top

Py:   re.findall(r"\d+", s)
来源：http://odi.shuidangran.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qvm.52xcode.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rto.cashguo.top

TS:   s.match(/\d+/g)
来源：http://wqq.dashuyun.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://osp.sufxvd.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wwn.chenzaomai.com

Ruby: s.scan(/\d+/)
来源：http://nnn.hysaishi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://egc.yanxiufei.cn

[I03] 提取捕获分组
来源：http://ujz.andypj.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://btf.andypj.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mhz.vehdjk.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://egk.mhx1999.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ssd.zdqjudy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xhi.vehdjk.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://igc.nanxinkj.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pgj.zhengqikj.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://uno.cucudq.cn

[I04] 正则替换
来源：http://atj.wangshuangyany.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://cgf.hesvh.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://srq.zhaomingkeji.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://miq.shanyushiyangkeji.top

TS:   s.replace(/\d+/g, "#")
来源：http://hzj.hnqzz.top

Java: s.replaceAll("\\d+", "#")
来源：http://jhc.sjlbkw.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://vjv.xuanzx.com

Ruby: s.gsub(/\d+/, "#")
来源：http://smk.yongpay.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vjg.epnwcf.com

[I05] 按正则拆分
来源：http://ual.nwbrower.top

Py:   re.split(r"\s*,\s*", s)
来源：http://cca.andypj.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wyk.zhoulong.xyz

JS:   s.split(/\s*,\s*/)
来源：http://toi.xuetiantiany.cn

TS:   s.split(/\s*,\s*/)
来源：http://jvm.cqqwz.cn

Java: s.split("\\s*,\\s*")
来源：http://vbd.cdnleiting.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://odi.yonumen.top

Ruby: s.split(/\s*,\s*/)
来源：http://fel.dashuyun.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rdz.zdqjudy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pay.sxryk.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://eyj.zdbjq.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rog.hammf.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hbg.meibo888.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zkb.jinghuilouyu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yec.guannengcc.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dxz.pengpengdd.cyou

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nza.svipenyu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://neh.feifeiyinyue.top

[I07] 忽略大小写与多行模式
来源：http://fsz.zhixingplan.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://sct.yj202588.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vds.ybcxt.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://elf.quarkkingdee.top

TS:   /error/gim
来源：http://ewn.zhoulong.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dsi.yuanzhike.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cca.yj20258888.top

Ruby: s.scan(/error/i)
来源：http://zhb.ppjwa.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pjz.yj202588.top

[I08] 贪婪与非贪婪匹配
来源：http://iyp.ybcxt.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ene.xuanzx.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ivm.fengsongda.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fxs.wangshuangyany.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qsk.hcnkem.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://qcb.daxiang520.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kyy.yvedp.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jfl.tian-w.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hzu.zhiwuduotai.top

================================================================================
来源：http://uer.yuanzhike.top

J. 日期与时间
来源：http://shw.redwolf501.top

================================================================================
来源：http://wsf.9152youxi.cn

[J01] 获取当前时间
来源：http://hdx.gogol.net.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://kpa.sufxvd.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xbr.yueranfly.top

JS:   new Date();  Date.now()
来源：http://hek.sufxvd.cn

TS:   new Date();  Date.now()
来源：http://iku.xuetiantiany.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://hck.epnwcf.com

Go:   time.Now()
来源：http://acg.svipenyu.cn

Ruby: Time.now
来源：http://sgf.bbcook.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bso.tanke756.top

[J02] 格式化输出
来源：http://cyz.fktsv.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ujx.yueranfly.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bjl.daria6918.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yzu.feifeiyinyue.top

TS:   d.toISOString()
来源：http://orh.epnwcf.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cqm.havefunace.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://osl.hfpthk.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://old.yonumen.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yqm.dianchejie.cn

[J03] 字符串解析为日期
来源：http://dtc.cucudq.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pvg.zhengqikj.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dee.52xcode.cn

JS:   new Date("2024-01-02")
来源：http://ucc.zdqjudy.top

TS:   new Date("2024-01-02")
来源：http://hen.shanyushiyangkeji.top

Java: LocalDate.parse("2024-01-02")
来源：http://gur.cdnleiting.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://idm.0kj1m.cn

Ruby: Date.parse("2024-01-02")
来源：http://ryu.fzhhl.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lub.kuanghao11.cn

[J04] 时间戳与日期互转
来源：http://ndz.zhijiandao.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jrl.fengsongda.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rbx.cashguo.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jdf.gotoacloud.top

TS:   Math.floor(Date.now() / 1000)
来源：http://cqi.9152youxi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lsq.fktsv.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gtk.uphjek.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gzj.jlsjyb.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zwn.redwolf501.top

[J05] 时间加减（加 7 天）
来源：http://yur.smart0.xyz

Py:   now + timedelta(days=7)
来源：http://fjj.sysykeji.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://lob.aibaodan.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fdn.iojbl.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cpr.kuanghao11.cn

Java: LocalDate.now().plusDays(7)
来源：http://ial.zhaomingkeji.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://psg.meibo888.top

Ruby: Time.now + 7 * 86400
来源：http://mcp.zhengqikj.top

C#:   DateTime.Now.AddDays(7)
来源：http://vjl.cqqwz.cn

[J06] 计算两时间之差
来源：http://hnw.fanxiaobao.xyz

Py:   (end - start).total_seconds()
来源：http://qzp.shanyushiyangtech.top

PHP:  $end->diff($start)->days;
来源：http://ycx.daria6918.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qrz.zdqjudy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dvn.daxiang520.top

Java: Duration.between(start, end).toSeconds()
来源：http://jud.cashguo.top

Go:   end.Sub(start).Hours()
来源：http://pun.chenlongwang.top

Ruby: end - start                 # 返回秒数
来源：http://bqj.sysykeji.top

C#:   (end - start).TotalSeconds
来源：http://nue.sweek.top

[J07] 比较两个日期
来源：http://xch.shanyushiyangtech.top

Py:   d1 < d2;  d1 == d2
来源：http://abx.xuanzx.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zeu.tarul.cn

JS:   d1.getTime() < d2.getTime()
来源：http://grd.zhongyouzk.top


<!-- 参考信息 -->
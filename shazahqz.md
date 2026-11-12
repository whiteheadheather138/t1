代发 wailian999

[G10] 访问控制
来源：http://dwm.tanke756.top

Py:   约定 _protected / __private（不强制）
来源：http://qmr.tanke756.top

PHP:  public / protected / private
来源：http://jvq.gogol.net.cn

JS:   #private 字段；其余公开
来源：http://vnd.havefunace.top

TS:   public / protected / private
来源：http://zoj.ydzc1.top

Java: public / protected / private / 默认包级
来源：http://xqc.zhengqikj.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://lhp.fanxiaobao.xyz

Ruby: public / protected / private
来源：http://idv.hcnkem.com

C#:   public / protected / private / internal
来源：http://okq.xylfe.cn

[G11] getter / setter
来源：http://psz.fengsongda.top

Py:   @property 与 @x.setter
来源：http://saq.sjlbkw.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://mnh.chenzaomai.com

JS:   get name() { return this._name; }
来源：http://nkr.zhaomingkeji.xyz

TS:   get name(): string { return this._name; }
来源：http://ppn.ppjwa.cn

Java: public String getName() { return name; }
来源：http://onk.shanyushiyangkeji.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://hgo.xuetiantiany.cn

Ruby: attr_accessor :name
来源：http://tet.zhiwuduotai.top

C#:   public string Name { get; set; }
来源：http://bwq.ppjwa.cn

[G12] 对象转字符串
来源：http://ryy.kuanghao11.cn

Py:   def __str__(self): return self.name
来源：http://awc.nanxuanxn.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://rft.yfazqb.com

JS:   toString() { return this.name; }
来源：http://ckb.hnqzz.top

TS:   toString(): string { return this.name; }
来源：http://iwa.vqdsnc.cn

Java: @Override public String toString() { return name; }
来源：http://blr.52xcode.cn

Go:   func (u User) String() string { return u.Name }
来源：http://pgq.ydzc1.top

Ruby: def to_s; @name; end
来源：http://yuz.uphjek.com

C#:   public override string ToString() => Name;
来源：http://ypq.yfazqb.com

[G13] 判断对象类型
来源：http://smn.ctjpmb.com

Py:   isinstance(u, User)
来源：http://ksv.sysykeji.top

PHP:  $u instanceof User
来源：http://flq.chenzaomai.com

JS:   u instanceof User
来源：http://zen.0kj1m.cn

TS:   u instanceof User
来源：http://ups.sjlbkw.cn

Java: u instanceof User
来源：http://wse.tarul.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://dlu.hesvh.cn

Ruby: u.is_a?(User)
来源：http://xxd.tianlin.xyz

C#:   u is User
来源：http://peu.gotoacloud.top

[G14] 数据类 / record
来源：http://neb.redwolf501.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wjr.yuxming.cn

PHP:  // 用 readonly 属性模拟
来源：http://yyx.xingfuxueyuan.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://ubg.cucudq.cn

TS:   type User = { name: string; age: number };
来源：http://pkw.havefunace.top

Java: record User(String name, int age) {}
来源：http://jxl.nwbrower.top

Go:   type User struct { Name string; Age int }
来源：http://muy.nwbrower.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ful.jinghuilouyu.cn

C#:   record User(string Name, int Age);
来源：http://gor.yongpay.top

[G15] 枚举
来源：http://hpi.aibaodan.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jur.sysykeji.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://xsy.shangyingyoupin.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://uhk.yonumen.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://elu.cqqwz.cn

Java: enum Color { RED, GREEN }
来源：http://aap.hfpthk.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gen.tarul.cn

Ruby: Color = %i[red green].freeze
来源：http://eeu.zhijiandao.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nbc.yangfankeji.com

[G16] 对象转数组 / 字典
来源：http://txd.ppjwa.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yfm.fehbvm.com

PHP:  get_object_vars($obj);
来源：http://kre.ppjwa.cn

JS:   Object.entries(obj)
来源：http://kwh.tanke756.top

TS:   Object.entries(obj)
来源：http://zds.guowangkeji.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://btf.fehbvm.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://ocx.nwbrower.top

Ruby: obj.instance_variables
来源：http://rgp.jinghuilouyu.cn

C#:   // 用反射或 System.Text.Json
来源：http://kgs.tanke756.top

================================================================================
来源：http://tdi.ydjk.org.cn

H. 异常与错误处理
来源：http://awt.andypj.xyz

================================================================================
来源：http://xgl.chenlongwang.top

[H01] try / catch 基础
来源：http://onw.yuxming.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nwi.fehbvm.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://srx.tanke756.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rkx.cheryme.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qzd.zhongyouzk.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ycu.gogol.net.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ltc.mhx1999.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://eoc.xylfe.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dnt.guannengcc.top

[H02] finally / ensure 收尾
来源：http://hhe.bbcook.cn

Py:   try: f()⏎finally: cleanup()
来源：http://orf.jinyuanbaomall.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://vjy.chenlongwang.top

JS:   try { f(); } finally { cleanup(); }
来源：http://nim.fengsongda.top

TS:   try { f(); } finally { cleanup(); }
来源：http://aqu.zhoulong.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://zzn.cucudq.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://yrw.jyoumei.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://lsi.dashuyun.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qgn.zhiwuduotai.top

[H03] 主动抛出异常
来源：http://pae.ywan-chungtsiang.top

Py:   raise ValueError("错误信息")
来源：http://xtp.aizwys.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ayr.shanyushiyangkeji.top

JS:   throw new Error("错误信息");
来源：http://cnz.316326.xyz

TS:   throw new Error("错误信息");
来源：http://bmd.zdbjq.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://nuk.svipenyu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hij.sufxvd.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wqa.shanyushiyangtech.top

C#:   throw new ArgumentException("错误信息");
来源：http://qqj.yfazqb.com

[H04] 自定义异常类型
来源：http://bfq.9152youxi.cn

Py:   class MyError(Exception): pass
来源：http://sbk.xuetiantiany.cn

PHP:  class MyError extends RuntimeException {}
来源：http://glx.guowangkeji.top

JS:   class MyError extends Error {}
来源：http://lkg.vqdsnc.cn

TS:   class MyError extends Error {}
来源：http://hon.9152youxi.cn

Java: class MyException extends RuntimeException {}
来源：http://ilc.gogol.net.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hbe.guowangkeji.top

Ruby: class MyError < StandardError; end
来源：http://qsv.guowangkeji.top

C#:   class MyException : Exception {}
来源：http://hdg.hnxiangtu.top

[H05] 捕获特定类型
来源：http://byl.xziqi.cn

Py:   except ValueError as e:
来源：http://dtw.shanyushiyangtech.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://htt.zhongyouzk.top

JS:   if (e instanceof TypeError) {}
来源：http://gvi.jyoumei.cn

TS:   if (e instanceof TypeError) {}
来源：http://gro.jqgfzy.top

Java: catch (IOException | SQLException e) {}
来源：http://zku.ctjpmb.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yom.yuanzhike.top

Ruby: rescue ArgumentError => e
来源：http://mhh.yueranfly.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blb.kuanghao11.cn

[H06] 可选值 / 空值安全访问
来源：http://itx.shanyushiyangkeji.top

Py:   value = d.get("k") or default
来源：http://eud.uphjek.com

PHP:  $v = $d["k"] ?? null;
来源：http://bjc.dianchejie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://snk.smart0.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://kvj.hammf.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fyl.sjlbkw.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://phn.hfpthk.cn

Ruby: d&.dig(:a, :b)
来源：http://pka.wangdashe.top

C#:   obj?.A?.B ?? default
来源：http://mpn.0kj1m.cn

[H07] 断言
来源：http://isl.iojbl.cn

Py:   assert x > 0, "必须为正"
来源：http://dvl.jqgfzy.top

PHP:  assert($x > 0);
来源：http://owl.jinqigufen.top

JS:   console.assert(x > 0);
来源：http://zfz.daxiang520.top

TS:   console.assert(x > 0);
来源：http://vlf.meibo888.top

Java: assert x > 0 : "必须为正";
来源：http://tli.zdbjq.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wyh.guannengcc.top

Ruby: raise "必须为正" unless x > 0
来源：http://owd.vqdsnc.cn

C#:   Debug.Assert(x > 0);
来源：http://sfb.zhiwuduotai.top

[H08] 获取错误信息与堆栈
来源：http://lrk.sysykeji.top

Py:   str(e);  traceback.format_exc()
来源：http://ppa.ppjwa.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qtz.ydjk.org.cn

JS:   e.message;  e.stack
来源：http://vsu.gaohongyu789.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://cku.xinyue.icu

Java: e.getMessage();  e.printStackTrace()
来源：http://kah.ppjwa.cn

Go:   err.Error()
来源：http://aje.zhijiandao.cn

Ruby: e.message;  e.backtrace
来源：http://czv.quarkkingdee.top

C#:   e.Message;  e.StackTrace
来源：http://nef.xingfuxueyuan.xyz

[H09] 带错误码的异常
来源：http://ddj.sufxvd.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vbb.zhongyouzk.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://msz.cqqwz.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mme.wangdashe.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zjg.daxiang520.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://riv.xingfuxueyuan.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qcp.aizwys.cn

Ruby: raise MyError.new("fail", 500)
来源：http://trm.zhongyouzk.top

C#:   // 自定义异常类中加 Code 属性
来源：http://kwr.yuxming.cn

[H10] 资源自动释放
来源：http://ngz.cqqwz.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://nhx.tian-w.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yiw.ybcxt.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://auj.redwolf501.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yrc.hesvh.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ggn.tanke756.top

Go:   defer f.Close()
来源：http://ccg.mhx1999.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://whz.havefunace.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sti.ppjwa.cn

================================================================================
来源：http://hpw.wangshuangyany.cn

I. 正则表达式
来源：http://yyj.xylfe.cn

================================================================================
来源：http://ttf.smart0.xyz

[I01] 判断是否匹配
来源：http://qeh.zhaomingkeji.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jih.yj202588.top

PHP:  preg_match('/\d+/', $s);
来源：http://uol.gaohongyu789.top

JS:   /\d+/.test(s)
来源：http://zzg.chenlongwang.top

TS:   /\d+/.test(s)
来源：http://ykm.hnxiangtu.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vcb.yfazqb.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vxw.wangdashe.top

Ruby: s.match?(/\d+/)
来源：http://bji.shanyushiyangtech.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ahh.haohaochexian.top

[I02] 提取所有匹配
来源：http://noq.ywan-chungtsiang.top

Py:   re.findall(r"\d+", s)
来源：http://yin.yangfankeji.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sdn.dianchejie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ila.ybcxt.top

TS:   s.match(/\d+/g)
来源：http://euu.gotoacloud.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nmv.316326.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jui.sysykeji.top

Ruby: s.scan(/\d+/)
来源：http://asa.pengpengdd.cyou

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://axe.guannengcc.top

[I03] 提取捕获分组
来源：http://ixe.jinyuanbaomall.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ggu.yfazqb.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vfj.guannengcc.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ozz.zdbjq.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mhb.jqgufenzy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dzz.yvedp.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gag.fanxiaobao.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gjb.jyoumei.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ujh.xuanzx.com

[I04] 正则替换
来源：http://iml.fengsongda.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ehn.jinghuilouyu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dii.shanyushiyangtech.top

JS:   s.replace(/\d+/g, "#")
来源：http://alx.jlsjyb.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xbo.nanxinkj.top

Java: s.replaceAll("\\d+", "#")
来源：http://dbr.xuanzx.com

Go:   re.ReplaceAllString(s, "#")
来源：http://ggm.hysaishi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://uej.jqgufenzy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rrt.ivvv.top

[I05] 按正则拆分
来源：http://yza.hnqzz.top

Py:   re.split(r"\s*,\s*", s)
来源：http://fyo.fehbvm.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zif.cashguo.top

JS:   s.split(/\s*,\s*/)
来源：http://ttt.jinyuanbaomall.cn

TS:   s.split(/\s*,\s*/)
来源：http://hrv.uphjek.com

Java: s.split("\\s*,\\s*")
来源：http://fzr.tian-w.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dgt.sufxvd.cn

Ruby: s.split(/\s*,\s*/)
来源：http://hyr.dashuyun.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lob.yonumen.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://eqj.yuanzhike.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vnu.zhengqikj.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ffo.yuanzhike.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qns.zhijiandao.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wsh.tarul.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://drq.cashguo.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ffw.iojbl.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yza.cqqwz.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ixe.ehwqpu.com

[I07] 忽略大小写与多行模式
来源：http://acb.epnwcf.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tgw.hnqzz.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vif.316326.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fpk.guowangkeji.top

TS:   /error/gim
来源：http://efw.nwbrower.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rss.ywan-chungtsiang.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://uzw.yj20258.top

Ruby: s.scan(/error/i)
来源：http://qzf.sjlbkw.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://svf.jinghuilouyu.cn

[I08] 贪婪与非贪婪匹配
来源：http://qle.hnxiangtu.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://aob.chenjidiqi.icu

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dqf.smart0.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://awt.sweek.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wvp.bjfxy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ehc.yueranfly.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fut.bbcook.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ipk.zhiwuduotai.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kob.gaohongyu789.top

================================================================================
来源：http://rkq.uphjek.com

J. 日期与时间
来源：http://tzr.pycfn.com

================================================================================
来源：http://aim.daxiang520.top

[J01] 获取当前时间
来源：http://zle.svipenyu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://eiq.jinyuanbaomall.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lmm.hfpthk.cn

JS:   new Date();  Date.now()
来源：http://fif.dashuyun.cn

TS:   new Date();  Date.now()
来源：http://fkn.chenlongwang.top

Java: LocalDateTime.now();  Instant.now()
来源：http://pmj.ydzc1.top

Go:   time.Now()
来源：http://xbv.jianghu66.top

Ruby: Time.now
来源：http://upz.hywenlv.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rrt.yangfankeji.com

[J02] 格式化输出
来源：http://wii.gzhubu.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rxu.jinghuilouyu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ezx.yj202588.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rja.epnwcf.com

TS:   d.toISOString()
来源：http://jxr.fehbvm.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zwl.hfpthk.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kfe.jinqigufen.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dyk.cucudq.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wkt.redwolf501.top

[J03] 字符串解析为日期
来源：http://fdx.wangdashe.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dtg.ctjpmb.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vjb.quarkkingdee.top

JS:   new Date("2024-01-02")
来源：http://wob.gogol.net.cn

TS:   new Date("2024-01-02")
来源：http://zxu.jinghuilouyu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://hbg.xylfe.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nwv.shanyushiyangtech.top

Ruby: Date.parse("2024-01-02")
来源：http://rnz.birdmap.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tsg.vehdjk.com

[J04] 时间戳与日期互转
来源：http://ygm.yonumen.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lwp.wangshuangyany.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mdz.vehdjk.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rvz.yfazqb.com

TS:   Math.floor(Date.now() / 1000)
来源：http://ixk.smart0.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://upl.bjfxy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ncd.hcnkem.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://var.sjlbkw.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hvj.cucudq.cn

[J05] 时间加减（加 7 天）
来源：http://bkq.feifeiyinyue.top

Py:   now + timedelta(days=7)
来源：http://xnn.andypj.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://bll.snrcjt.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bxt.ybcxt.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://aub.cucudq.cn

Java: LocalDate.now().plusDays(7)
来源：http://bdp.cucudq.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vch.ybcxt.top

Ruby: Time.now + 7 * 86400
来源：http://kft.zdqjudy.top

C#:   DateTime.Now.AddDays(7)
来源：http://bdv.vehdjk.com

[J06] 计算两时间之差
来源：http://czg.tian-w.cn

Py:   (end - start).total_seconds()
来源：http://tgy.nwbrower.top

PHP:  $end->diff($start)->days;
来源：http://rhz.hfpthk.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://grz.hesvh.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://aub.zdbjq.cn

Java: Duration.between(start, end).toSeconds()
来源：http://fro.shzxlz.cn

Go:   end.Sub(start).Hours()
来源：http://zkv.bbcook.cn

Ruby: end - start                 # 返回秒数
来源：http://swf.tian-w.cn

C#:   (end - start).TotalSeconds
来源：http://exr.hfpthk.cn

[J07] 比较两个日期
来源：http://wre.aizwys.cn

Py:   d1 < d2;  d1 == d2
来源：http://pjv.yueranfly.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gts.jqgfzy.top

JS:   d1.getTime() < d2.getTime()
来源：http://tkl.meibo888.top

TS:   d1.getTime() < d2.getTime()
来源：http://kre.ydzc1.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://inv.yanxiufei.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ubq.0kj1m.cn

Ruby: d1 < d2;  d1 == d2
来源：http://pro.nanxinkj.top

C#:   d1 < d2;  d1 == d2
来源：http://hly.vqdsnc.cn

[J08] 提取年月日与星期
来源：http://djz.bjfxy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://glo.ivvv.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fim.yj20258.top


<!-- 参考信息 -->
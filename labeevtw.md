代发 wailian999

C#:   public / protected / private / internal
来源：http://meo.hongshengwenyu.top

[G11] getter / setter
来源：http://mlp.jianghu66.top

Py:   @property 与 @x.setter
来源：http://rgp.guowangkeji.top

PHP:  public function getName(): string { return $this->name; }
来源：http://lgp.epnwcf.com

JS:   get name() { return this._name; }
来源：http://oli.jinyuanbaomall.cn

TS:   get name(): string { return this._name; }
来源：http://wup.nwbrower.top

Java: public String getName() { return name; }
来源：http://ydj.chenlongwang.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://vmw.gotoacloud.top

Ruby: attr_accessor :name
来源：http://cyh.hammf.cn

C#:   public string Name { get; set; }
来源：http://daf.yueranfly.top

[G12] 对象转字符串
来源：http://vkb.jyoumei.cn

Py:   def __str__(self): return self.name
来源：http://nul.nanxinkj.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://zbs.xuanzx.com

JS:   toString() { return this.name; }
来源：http://ecl.316326.xyz

TS:   toString(): string { return this.name; }
来源：http://txt.shuidangran.top

Java: @Override public String toString() { return name; }
来源：http://bps.gzhubu.top

Go:   func (u User) String() string { return u.Name }
来源：http://cup.shanyushiyangkeji.top

Ruby: def to_s; @name; end
来源：http://nhk.guowangkeji.top

C#:   public override string ToString() => Name;
来源：http://fcx.9152youxi.cn

[G13] 判断对象类型
来源：http://bmy.cucudq.cn

Py:   isinstance(u, User)
来源：http://axe.zhengqikj.top

PHP:  $u instanceof User
来源：http://alz.yueranfly.top

JS:   u instanceof User
来源：http://znj.ybcxt.top

TS:   u instanceof User
来源：http://hoe.cheryme.top

Java: u instanceof User
来源：http://ncj.hongshengwenyu.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://slj.ydzc1.top

Ruby: u.is_a?(User)
来源：http://qkr.hammf.cn

C#:   u is User
来源：http://azg.hfpthk.cn

[G14] 数据类 / record
来源：http://zkp.shanyushiyangkeji.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xgq.meibo888.top

PHP:  // 用 readonly 属性模拟
来源：http://zwo.zdqjudy.top

JS:   // 无内置：普通类或对象字面量
来源：http://eac.yueranfly.top

TS:   type User = { name: string; age: number };
来源：http://ltw.hnqzz.top

Java: record User(String name, int age) {}
来源：http://qiw.iojbl.cn

Go:   type User struct { Name string; Age int }
来源：http://ede.ydzc1.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://neg.meibo888.top

C#:   record User(string Name, int Age);
来源：http://ebx.svipenyu.cn

[G15] 枚举
来源：http://zef.aibaodan.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://eoq.guowangkeji.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ndd.havefunace.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jdd.guowangkeji.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cru.yvedp.cn

Java: enum Color { RED, GREEN }
来源：http://eos.gogol.net.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yhl.nwbrower.top

Ruby: Color = %i[red green].freeze
来源：http://qqp.fanxiaobao.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qpi.jlsjyb.cn

[G16] 对象转数组 / 字典
来源：http://nhl.haohaochexian.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ggy.hywenlv.cn

PHP:  get_object_vars($obj);
来源：http://qlw.meibo888.top

JS:   Object.entries(obj)
来源：http://obz.sweek.top

TS:   Object.entries(obj)
来源：http://jzc.xziqi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wds.uphjek.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://jqd.redwolf501.top

Ruby: obj.instance_variables
来源：http://jkr.chenzaomai.com

C#:   // 用反射或 System.Text.Json
来源：http://mba.nwbrower.top

================================================================================
来源：http://upb.zdqjudy.top

H. 异常与错误处理
来源：http://bke.yj20258.top

================================================================================
来源：http://jfo.hnqzz.top

[H01] try / catch 基础
来源：http://kmx.sjlbkw.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zva.jqgufenzy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tnu.hfpthk.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://slu.jianghu66.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://plv.guannengcc.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zhf.zhixingplan.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ozg.xuanzx.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hci.hammf.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://asq.jqgufenzy.top

[H02] finally / ensure 收尾
来源：http://tmn.shuidangran.top

Py:   try: f()⏎finally: cleanup()
来源：http://max.chenzaomai.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://swp.ehwqpu.com

JS:   try { f(); } finally { cleanup(); }
来源：http://zur.zhongyouzk.top

TS:   try { f(); } finally { cleanup(); }
来源：http://jmz.ydjk.org.cn

Java: try { f(); } finally { cleanup(); }
来源：http://bfd.0kj1m.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://csv.ppjwa.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://cgn.ydzc1.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://fln.xziqi.cn

[H03] 主动抛出异常
来源：http://wlk.tianlin.xyz

Py:   raise ValueError("错误信息")
来源：http://bav.shzxlz.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://uwg.tianlin.xyz

JS:   throw new Error("错误信息");
来源：http://ddi.wangdashe.top

TS:   throw new Error("错误信息");
来源：http://wci.snrcjt.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://kho.wangshuangyany.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xqh.bbcook.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://yab.svipenyu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://zxb.hammf.cn

[H04] 自定义异常类型
来源：http://xxo.ydzc1.top

Py:   class MyError(Exception): pass
来源：http://vim.kuanghao11.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ejw.tianlin.xyz

JS:   class MyError extends Error {}
来源：http://cpa.wangshuangyany.cn

TS:   class MyError extends Error {}
来源：http://hwx.gotoacloud.top

Java: class MyException extends RuntimeException {}
来源：http://soe.shanyushiyangtech.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vak.nanxinkj.top

Ruby: class MyError < StandardError; end
来源：http://lam.sjlbkw.cn

C#:   class MyException : Exception {}
来源：http://bou.zhengqikj.top

[H05] 捕获特定类型
来源：http://qzi.zhaomingkeji.xyz

Py:   except ValueError as e:
来源：http://yza.zhaomingkeji.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xsc.hnqzz.top

JS:   if (e instanceof TypeError) {}
来源：http://dhp.kuanghao11.cn

TS:   if (e instanceof TypeError) {}
来源：http://dxb.meibo888.top

Java: catch (IOException | SQLException e) {}
来源：http://pzf.yj20258.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cub.dashuyun.cn

Ruby: rescue ArgumentError => e
来源：http://twb.zhixingplan.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ihx.epnwcf.com

[H06] 可选值 / 空值安全访问
来源：http://zlq.tanke756.top

Py:   value = d.get("k") or default
来源：http://vsf.chenlongwang.top

PHP:  $v = $d["k"] ?? null;
来源：http://pik.kuanghao11.cn

JS:   obj?.a?.b;  d ?? default
来源：http://knq.cheryme.top

TS:   obj?.a?.b;  d ?? default
来源：http://dhf.ybcxt.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vqc.xziqi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://kko.chenlongwang.top

Ruby: d&.dig(:a, :b)
来源：http://rah.wangshuangyany.cn

C#:   obj?.A?.B ?? default
来源：http://cox.nanxinkj.top

[H07] 断言
来源：http://jyl.hcnkem.com

Py:   assert x > 0, "必须为正"
来源：http://tar.chenjidiqi.icu

PHP:  assert($x > 0);
来源：http://zbr.yangfankeji.com

JS:   console.assert(x > 0);
来源：http://nqg.cdnleiting.top

TS:   console.assert(x > 0);
来源：http://dus.dashuyun.cn

Java: assert x > 0 : "必须为正";
来源：http://rud.iojbl.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kyj.cheryme.top

Ruby: raise "必须为正" unless x > 0
来源：http://nwm.chenjidiqi.icu

C#:   Debug.Assert(x > 0);
来源：http://vdo.havefunace.top

[H08] 获取错误信息与堆栈
来源：http://ape.daria6918.cn

Py:   str(e);  traceback.format_exc()
来源：http://ajo.nwbrower.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://adb.yj20258.top

JS:   e.message;  e.stack
来源：http://edf.c1oappe.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://eau.svipenyu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://fax.cashguo.top

Go:   err.Error()
来源：http://fxi.zdqjudy.top

Ruby: e.message;  e.backtrace
来源：http://gua.cashguo.top

C#:   e.Message;  e.StackTrace
来源：http://cqi.fehbvm.com

[H09] 带错误码的异常
来源：http://kkh.zhoulong.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rdx.9152youxi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://fty.hysaishi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ren.tianlin.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://acc.sweek.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://txa.sxryk.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yda.tanke756.top

Ruby: raise MyError.new("fail", 500)
来源：http://kdf.ivvv.top

C#:   // 自定义异常类中加 Code 属性
来源：http://dev.dianchejie.cn

[H10] 资源自动释放
来源：http://uut.yfazqb.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://rbm.shangyingyoupin.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ogg.meibo888.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://uln.daxiang520.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ehi.tanke756.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dfr.bbcook.cn

Go:   defer f.Close()
来源：http://yyc.zycfv.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pdy.snrcjt.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ear.xylfe.cn

================================================================================
来源：http://oux.jqgufenzy.top

I. 正则表达式
来源：http://iey.ctjpmb.com

================================================================================
来源：http://ovo.ydzc1.top

[I01] 判断是否匹配
来源：http://yfc.xinyue.icu

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://svp.yuanzhike.top

PHP:  preg_match('/\d+/', $s);
来源：http://lhd.quarkkingdee.top

JS:   /\d+/.test(s)
来源：http://orx.yj20258.top

TS:   /\d+/.test(s)
来源：http://nwl.cheryme.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pkx.jyoumei.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ocx.cqqwz.cn

Ruby: s.match?(/\d+/)
来源：http://bmj.wangshuangyany.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xpb.jianghu66.top

[I02] 提取所有匹配
来源：http://ayp.chenjidiqi.icu

Py:   re.findall(r"\d+", s)
来源：http://frd.cheryme.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://atb.smart0.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://iyj.jinghuilouyu.cn

TS:   s.match(/\d+/g)
来源：http://osc.aibaodan.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zsh.yonumen.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ebe.zhijiandao.cn

Ruby: s.scan(/\d+/)
来源：http://tup.xinyue.icu

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vua.hesvh.cn

[I03] 提取捕获分组
来源：http://khe.cashguo.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xrp.ivvv.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://evr.c1oappe.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://aln.ppjwa.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hzt.quarkkingdee.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://uay.chenlongwang.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zda.0kj1m.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yyi.hfpthk.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qbk.hnxiangtu.top

[I04] 正则替换
来源：http://cft.xziqi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://tds.yfazqb.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://azo.zdqjudy.top

JS:   s.replace(/\d+/g, "#")
来源：http://qrx.jqgfzy.top

TS:   s.replace(/\d+/g, "#")
来源：http://qnl.xziqi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ijx.yonumen.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ffh.jinqigufen.top

Ruby: s.gsub(/\d+/, "#")
来源：http://qxv.wangshuangyany.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fsm.tian-w.cn

[I05] 按正则拆分
来源：http://jop.xuetiantiany.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://jtp.havefunace.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://glm.wangshuangyany.cn

JS:   s.split(/\s*,\s*/)
来源：http://uad.sufxvd.cn

TS:   s.split(/\s*,\s*/)
来源：http://dbs.snrcjt.cn

Java: s.split("\\s*,\\s*")
来源：http://hqe.hongshengwenyu.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hue.shanyushiyangtech.top

Ruby: s.split(/\s*,\s*/)
来源：http://kei.gzhubu.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dfn.gzhubu.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sch.gaohongyu789.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://keo.shanyushiyangkeji.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mlu.meibo888.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cll.hfpthk.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://trz.shzxlz.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mpx.meibo888.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://erc.sufxvd.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dge.dianchejie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lod.kuanghao11.cn

[I07] 忽略大小写与多行模式
来源：http://kvn.ctjpmb.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://exr.hnqzz.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ohm.yangfankeji.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fet.sufxvd.cn

TS:   /error/gim
来源：http://uww.svipenyu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mpk.nanxinkj.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ddd.tian-w.cn

Ruby: s.scan(/error/i)
来源：http://qvr.52xcode.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vxu.sufxvd.cn

[I08] 贪婪与非贪婪匹配
来源：http://tnj.yueranfly.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hfb.fengsongda.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qre.chenzaomai.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kmg.yfazqb.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qvm.xuetiantiany.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://brk.bbcook.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wqz.kuanghao11.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qwc.gzhubu.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rwu.meibo888.top

================================================================================
来源：http://sin.tarul.cn

J. 日期与时间
来源：http://gzc.xziqi.cn

================================================================================
来源：http://qpk.yonumen.top

[J01] 获取当前时间
来源：http://bvs.daxiang520.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://dkl.hywenlv.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gwt.sjlbkw.cn

JS:   new Date();  Date.now()
来源：http://qhw.yj20258888.top

TS:   new Date();  Date.now()
来源：http://hbw.cashguo.top

Java: LocalDateTime.now();  Instant.now()
来源：http://jyd.ppjwa.cn

Go:   time.Now()
来源：http://sev.sysykeji.top

Ruby: Time.now
来源：http://duq.ydzc1.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vln.zycfv.cn

[J02] 格式化输出
来源：http://hcc.yuxming.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pek.jinqigufen.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bmi.zhengqikj.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://osn.316326.xyz

TS:   d.toISOString()
来源：http://xbb.daxiang520.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://boa.iojbl.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hrl.ctjpmb.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ggu.sjlbkw.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xoh.bjfxy.top

[J03] 字符串解析为日期
来源：http://mmi.sxryk.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://uhn.yuanzhike.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://frx.tian-w.cn

JS:   new Date("2024-01-02")
来源：http://ttc.xuanzx.com

TS:   new Date("2024-01-02")
来源：http://awi.hesvh.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fwo.dashuyun.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://grw.jinqigufen.top

Ruby: Date.parse("2024-01-02")
来源：http://ofs.daria6918.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gih.daria6918.cn

[J04] 时间戳与日期互转
来源：http://zjo.cheryme.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://svf.xinyue.icu

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qzc.nwbrower.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nfb.sysykeji.top

TS:   Math.floor(Date.now() / 1000)
来源：http://cqe.sysykeji.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://riy.gzhubu.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wxu.fehbvm.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wpj.jinqigufen.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ncv.hcnkem.com

[J05] 时间加减（加 7 天）
来源：http://sho.hywenlv.cn

Py:   now + timedelta(days=7)
来源：http://gnx.jinqigfzy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ced.shangyingyoupin.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pxe.zhiwuduotai.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qru.hammf.cn

Java: LocalDate.now().plusDays(7)
来源：http://jjt.mhx1999.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kra.kuanghao11.cn

Ruby: Time.now + 7 * 86400
来源：http://ksd.fanxiaobao.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://ysi.fengsongda.top

[J06] 计算两时间之差
来源：http://vfx.shanyushiyangkeji.top

Py:   (end - start).total_seconds()
来源：http://rbt.quarkkingdee.top

PHP:  $end->diff($start)->days;
来源：http://kxo.feifeiyinyue.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://psf.aibaodan.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ptp.sufxvd.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bwn.aizwys.cn

Go:   end.Sub(start).Hours()
来源：http://hyv.svipenyu.cn

Ruby: end - start                 # 返回秒数
来源：http://fcn.vqdsnc.cn

C#:   (end - start).TotalSeconds
来源：http://fjt.jinqigufen.top

[J07] 比较两个日期
来源：http://sbe.sufxvd.cn

Py:   d1 < d2;  d1 == d2
来源：http://bch.fehbvm.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jac.andypj.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://xaq.xinyue.icu

TS:   d1.getTime() < d2.getTime()
来源：http://uvy.sysykeji.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://icn.jinyuanbaomall.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xhv.52xcode.cn

Ruby: d1 < d2;  d1 == d2
来源：http://xwt.havefunace.top

C#:   d1 < d2;  d1 == d2
来源：http://xbv.yfazqb.com

[J08] 提取年月日与星期
来源：http://jko.kuanghao11.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://svs.svipenyu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cqy.gzhubu.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zxh.bjfxy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://aeq.tanke756.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dmv.fktsv.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sca.cucudq.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://iuw.tarul.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://oum.ybcxt.top

[J09] 时区处理
来源：http://zow.zhiwuduotai.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tqi.zdqjudy.top


<!-- 参考信息 -->
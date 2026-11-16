代发 wailian999

JS:   get name() { return this._name; }
来源：http://goj.daria6918.cn

TS:   get name(): string { return this._name; }
来源：http://lvx.316326.xyz

Java: public String getName() { return name; }
来源：http://nbh.hfpthk.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://lls.zhijiandao.cn

Ruby: attr_accessor :name
来源：http://rzf.yanxiufei.cn

C#:   public string Name { get; set; }
来源：http://tys.jqgfzy.top

[G12] 对象转字符串
来源：http://pub.cdnleiting.top

Py:   def __str__(self): return self.name
来源：http://loh.zhaomingkeji.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://qoq.cqqwz.cn

JS:   toString() { return this.name; }
来源：http://tnu.jinqigfzy.top

TS:   toString(): string { return this.name; }
来源：http://auf.jqgufenzy.top

Java: @Override public String toString() { return name; }
来源：http://xur.sjlbkw.cn

Go:   func (u User) String() string { return u.Name }
来源：http://iji.xylfe.cn

Ruby: def to_s; @name; end
来源：http://qem.hfpthk.cn

C#:   public override string ToString() => Name;
来源：http://gys.hammf.cn

[G13] 判断对象类型
来源：http://asp.shzxlz.cn

Py:   isinstance(u, User)
来源：http://nsk.nanxuanxn.top

PHP:  $u instanceof User
来源：http://qnx.bjfxy.top

JS:   u instanceof User
来源：http://npt.fengsongda.top

TS:   u instanceof User
来源：http://cbc.havefunace.top

Java: u instanceof User
来源：http://dqe.nwbrower.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://owr.xziqi.cn

Ruby: u.is_a?(User)
来源：http://syk.jiagoushi.top

C#:   u is User
来源：http://dsy.jinyuanbaomall.cn

[G14] 数据类 / record
来源：http://hvg.316326.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://drw.wangshuangyany.cn

PHP:  // 用 readonly 属性模拟
来源：http://hpl.yanxiufei.cn

JS:   // 无内置：普通类或对象字面量
来源：http://yyu.tarul.cn

TS:   type User = { name: string; age: number };
来源：http://oip.daria6918.cn

Java: record User(String name, int age) {}
来源：http://vlz.gzhubu.top

Go:   type User struct { Name string; Age int }
来源：http://wum.0kj1m.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://unb.ybcxt.top

C#:   record User(string Name, int Age);
来源：http://qkc.zhongyouzk.top

[G15] 枚举
来源：http://xyl.tianlin.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pqh.jinqigfzy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://bci.jianghu66.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pcp.9152youxi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xwh.hammf.cn

Java: enum Color { RED, GREEN }
来源：http://msh.yangfankeji.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ogr.9152youxi.cn

Ruby: Color = %i[red green].freeze
来源：http://sbw.pycfn.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yku.yongpay.top

[G16] 对象转数组 / 字典
来源：http://ltn.hongshengwenyu.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jqa.hywenlv.cn

PHP:  get_object_vars($obj);
来源：http://ljt.zhixingplan.top

JS:   Object.entries(obj)
来源：http://sqs.sweek.top

TS:   Object.entries(obj)
来源：http://gpa.nanxinkj.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://loi.gotoacloud.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://qdc.jlsjyb.cn

Ruby: obj.instance_variables
来源：http://oqk.fktsv.cn

C#:   // 用反射或 System.Text.Json
来源：http://ksv.nanxinkj.top

================================================================================
来源：http://dzu.yonumen.top

H. 异常与错误处理
来源：http://zvw.yonumen.top

================================================================================
来源：http://xzg.mhx1999.top

[H01] try / catch 基础
来源：http://liq.yuanzhike.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vec.9152youxi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ufq.fanxiaobao.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kkc.ydjk.org.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://met.ybcxt.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lze.fktsv.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hjh.tianlin.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ehc.ybcxt.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://srd.feifeiyinyue.top

[H02] finally / ensure 收尾
来源：http://uih.yanxiufei.cn

Py:   try: f()⏎finally: cleanup()
来源：http://gpu.smart0.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://xer.ywan-chungtsiang.top

JS:   try { f(); } finally { cleanup(); }
来源：http://kqk.gaohongyu789.top

TS:   try { f(); } finally { cleanup(); }
来源：http://gma.shanyushiyangtech.top

Java: try { f(); } finally { cleanup(); }
来源：http://ngh.pycfn.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://hup.ctjpmb.com

Ruby: begin; f; ensure; cleanup; end
来源：http://ngg.gaohongyu789.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://gey.hcnkem.com

[H03] 主动抛出异常
来源：http://ilm.yueranfly.top

Py:   raise ValueError("错误信息")
来源：http://oxq.epnwcf.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jmd.cheryme.top

JS:   throw new Error("错误信息");
来源：http://sdc.gogol.net.cn

TS:   throw new Error("错误信息");
来源：http://wpu.jinyuanbaomall.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ehr.daxiang520.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rfm.shangyingyoupin.top

Ruby: raise ArgumentError, "错误信息"
来源：http://qbg.ctjpmb.com

C#:   throw new ArgumentException("错误信息");
来源：http://qew.svipenyu.cn

[H04] 自定义异常类型
来源：http://gmr.hongshengwenyu.top

Py:   class MyError(Exception): pass
来源：http://opt.dianchejie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://beu.shanyushiyangkeji.top

JS:   class MyError extends Error {}
来源：http://uqq.nwbrower.top

TS:   class MyError extends Error {}
来源：http://sap.vehdjk.com

Java: class MyException extends RuntimeException {}
来源：http://dhh.shzxlz.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hxr.andypj.xyz

Ruby: class MyError < StandardError; end
来源：http://eni.fehbvm.com

C#:   class MyException : Exception {}
来源：http://ddl.chenlongwang.top

[H05] 捕获特定类型
来源：http://evj.wangshuangyany.cn

Py:   except ValueError as e:
来源：http://tgt.haohaochexian.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jnk.fktsv.cn

JS:   if (e instanceof TypeError) {}
来源：http://piz.jinghuilouyu.cn

TS:   if (e instanceof TypeError) {}
来源：http://jsi.aibaodan.cn

Java: catch (IOException | SQLException e) {}
来源：http://kmi.bbcook.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dfa.hywenlv.cn

Ruby: rescue ArgumentError => e
来源：http://ubv.nwbrower.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fnh.sxryk.cn

[H06] 可选值 / 空值安全访问
来源：http://skh.cucudq.cn

Py:   value = d.get("k") or default
来源：http://qel.chenlongwang.top

PHP:  $v = $d["k"] ?? null;
来源：http://ldt.wangdashe.top

JS:   obj?.a?.b;  d ?? default
来源：http://htj.sweek.top

TS:   obj?.a?.b;  d ?? default
来源：http://mjc.chenlongwang.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tkt.snrcjt.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://fnt.zhaomingkeji.xyz

Ruby: d&.dig(:a, :b)
来源：http://kfa.jqgfzy.top

C#:   obj?.A?.B ?? default
来源：http://cee.zhengqikj.top

[H07] 断言
来源：http://opd.hnxiangtu.top

Py:   assert x > 0, "必须为正"
来源：http://xex.hesvh.cn

PHP:  assert($x > 0);
来源：http://zec.chenlongwang.top

JS:   console.assert(x > 0);
来源：http://ilk.birdmap.top

TS:   console.assert(x > 0);
来源：http://uup.zhengqikj.top

Java: assert x > 0 : "必须为正";
来源：http://ksh.daxiang520.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jex.cdnleiting.top

Ruby: raise "必须为正" unless x > 0
来源：http://vce.hnqzz.top

C#:   Debug.Assert(x > 0);
来源：http://hto.ydzc1.top

[H08] 获取错误信息与堆栈
来源：http://bqz.yj20258888.top

Py:   str(e);  traceback.format_exc()
来源：http://yqo.yj20258888.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bfx.9152youxi.cn

JS:   e.message;  e.stack
来源：http://ohi.ctjpmb.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://mtz.bjfxy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://nhh.jianghu66.top

Go:   err.Error()
来源：http://pee.yanxiufei.cn

Ruby: e.message;  e.backtrace
来源：http://ree.jinqigfzy.top

C#:   e.Message;  e.StackTrace
来源：http://tsy.jinyuanbaomall.cn

[H09] 带错误码的异常
来源：http://oab.yj20258888.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://stt.ydjk.org.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://bpg.ydjk.org.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ijn.meibo888.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ddu.sufxvd.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dzu.birdmap.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nqw.c1oappe.top

Ruby: raise MyError.new("fail", 500)
来源：http://vtx.cucudq.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://yug.smart0.xyz

[H10] 资源自动释放
来源：http://gla.sweek.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://gda.yfazqb.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vcl.9152youxi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qou.0kj1m.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://slk.hnqzz.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tmb.pycfn.com

Go:   defer f.Close()
来源：http://vhl.xingfuxueyuan.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vjo.nanxinkj.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qar.andypj.xyz

================================================================================
来源：http://rty.yfazqb.com

I. 正则表达式
来源：http://mxn.xuetiantiany.cn

================================================================================
来源：http://hha.fktsv.cn

[I01] 判断是否匹配
来源：http://uuy.fengsongda.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://sci.yvedp.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ptq.vqdsnc.cn

JS:   /\d+/.test(s)
来源：http://twb.9152youxi.cn

TS:   /\d+/.test(s)
来源：http://dvu.vehdjk.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lku.tarul.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rfu.xuetiantiany.cn

Ruby: s.match?(/\d+/)
来源：http://eir.cucudq.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qqb.chenlongwang.top

[I02] 提取所有匹配
来源：http://arr.fktsv.cn

Py:   re.findall(r"\d+", s)
来源：http://bgx.fehbvm.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nhp.xuanzx.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://iqv.ppjwa.cn

TS:   s.match(/\d+/g)
来源：http://mqk.cheryme.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://krw.pengpengdd.cyou

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bia.quarkkingdee.top

Ruby: s.scan(/\d+/)
来源：http://tfn.bjfxy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ilh.pengpengdd.cyou

[I03] 提取捕获分组
来源：http://tuz.shuidangran.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://aem.xylfe.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pmu.yuanzhike.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://twp.316326.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rhj.9152youxi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cyy.fktsv.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zue.guowangkeji.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://sfb.guowangkeji.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lyo.cdnleiting.top

[I04] 正则替换
来源：http://fwi.xinyue.icu

Py:   re.sub(r"\d+", "#", s)
来源：http://zoc.xinyue.icu

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hoy.hesvh.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ymg.yj20258888.top

TS:   s.replace(/\d+/g, "#")
来源：http://gxs.yj20258.top

Java: s.replaceAll("\\d+", "#")
来源：http://pdm.shanyushiyangkeji.top

Go:   re.ReplaceAllString(s, "#")
来源：http://dew.yangfankeji.com

Ruby: s.gsub(/\d+/, "#")
来源：http://oxz.52xcode.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kmv.jinqigfzy.top

[I05] 按正则拆分
来源：http://rjf.tianlin.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://eui.ywan-chungtsiang.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gjl.zhiwuduotai.top

JS:   s.split(/\s*,\s*/)
来源：http://oji.ppjwa.cn

TS:   s.split(/\s*,\s*/)
来源：http://uyz.ywan-chungtsiang.top

Java: s.split("\\s*,\\s*")
来源：http://mny.shangyingyoupin.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vct.havefunace.top

Ruby: s.split(/\s*,\s*/)
来源：http://aju.cashguo.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mia.aibaodan.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://leo.chenjidiqi.icu

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://syk.ppjwa.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://khs.sufxvd.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://soj.epnwcf.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ygb.hcnkem.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mhl.hcnkem.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fpv.ywan-chungtsiang.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cnu.ybcxt.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nms.xinyue.icu

[I07] 忽略大小写与多行模式
来源：http://fjv.kuanghao11.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pso.hnxiangtu.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zzp.fengsongda.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://weo.wangdashe.top

TS:   /error/gim
来源：http://saf.316326.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ogz.52xcode.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://aqd.bjfxy.top

Ruby: s.scan(/error/i)
来源：http://hfk.bjfxy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mrs.yuxming.cn

[I08] 贪婪与非贪婪匹配
来源：http://xzc.cheryme.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yox.xingfuxueyuan.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tna.cashguo.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zor.hnqzz.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xce.xinyue.icu

Java: Pattern.compile("<b>.*?</b>")
来源：http://fue.andypj.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kik.wangshuangyany.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cuw.zhongyouzk.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ghp.hysaishi.cn

================================================================================
来源：http://uoh.guowangkeji.top

J. 日期与时间
来源：http://sak.pengpengdd.cyou

================================================================================
来源：http://wdn.guowangkeji.top

[J01] 获取当前时间
来源：http://kgk.jinghuilouyu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://rhv.hongshengwenyu.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hai.epnwcf.com

JS:   new Date();  Date.now()
来源：http://trr.guannengcc.top

TS:   new Date();  Date.now()
来源：http://ipr.sufxvd.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ogi.tarul.cn

Go:   time.Now()
来源：http://git.snrcjt.cn

Ruby: Time.now
来源：http://sht.havefunace.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://seh.yangfankeji.com

[J02] 格式化输出
来源：http://nmn.zhixingplan.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://frv.cqqwz.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gja.andypj.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kit.gogol.net.cn

TS:   d.toISOString()
来源：http://cjt.hammf.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kim.uphjek.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://crp.0kj1m.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ruv.yj202588.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wdh.xuanzx.com

[J03] 字符串解析为日期
来源：http://hsx.zdqjudy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mlv.nanxuanxn.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tnj.uphjek.com

JS:   new Date("2024-01-02")
来源：http://mvt.hywenlv.cn

TS:   new Date("2024-01-02")
来源：http://yie.fzhhl.top

Java: LocalDate.parse("2024-01-02")
来源：http://aqj.vehdjk.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rzo.shanyushiyangkeji.top

Ruby: Date.parse("2024-01-02")
来源：http://pqm.cdnleiting.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ldn.fzhhl.top

[J04] 时间戳与日期互转
来源：http://rlf.mhx1999.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gvd.andypj.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kwq.sjlbkw.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jnp.uphjek.com

TS:   Math.floor(Date.now() / 1000)
来源：http://why.yj20258.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ijk.fehbvm.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ngg.zdbjq.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dsf.ehwqpu.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://iac.316326.xyz

[J05] 时间加减（加 7 天）
来源：http://fip.wangshuangyany.cn

Py:   now + timedelta(days=7)
来源：http://mav.gzhubu.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://vpv.sufxvd.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jwh.52xcode.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://egt.tian-w.cn

Java: LocalDate.now().plusDays(7)
来源：http://xza.fengsongda.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nws.yangfankeji.com

Ruby: Time.now + 7 * 86400
来源：http://fzk.shanyushiyangtech.top

C#:   DateTime.Now.AddDays(7)
来源：http://zwo.hammf.cn

[J06] 计算两时间之差
来源：http://elp.havefunace.top

Py:   (end - start).total_seconds()
来源：http://ivn.shangyingyoupin.top

PHP:  $end->diff($start)->days;
来源：http://vmx.chenjidiqi.icu

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nsb.zhoulong.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://aqe.jinqigfzy.top

Java: Duration.between(start, end).toSeconds()
来源：http://ajl.zhoulong.xyz

Go:   end.Sub(start).Hours()
来源：http://skx.xuetiantiany.cn

Ruby: end - start                 # 返回秒数
来源：http://yon.chenlongwang.top

C#:   (end - start).TotalSeconds
来源：http://exf.yonumen.top

[J07] 比较两个日期
来源：http://uul.quarkkingdee.top

Py:   d1 < d2;  d1 == d2
来源：http://mcs.zhengqikj.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qmo.ydjk.org.cn

JS:   d1.getTime() < d2.getTime()
来源：http://gun.yj202588.top

TS:   d1.getTime() < d2.getTime()
来源：http://rel.yj20258888.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://byk.jinqigfzy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wiu.jqgfzy.top

Ruby: d1 < d2;  d1 == d2
来源：http://kjx.yj202588.top

C#:   d1 < d2;  d1 == d2
来源：http://rzo.xinyue.icu

[J08] 提取年月日与星期
来源：http://owk.nwbrower.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://txo.sjlbkw.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vxd.fktsv.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://okz.ehwqpu.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fuj.hysaishi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jhb.cucudq.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sjd.yj20258.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zbj.jqgufenzy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ygl.jinqigufen.top

[J09] 时区处理
来源：http://rgc.nwbrower.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jsv.hongshengwenyu.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wve.hongshengwenyu.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ozr.yuanzhike.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vln.kuanghao11.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gxh.shanyushiyangkeji.top


<!-- 参考信息 -->
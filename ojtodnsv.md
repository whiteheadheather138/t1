代发 wailian999

JS:   get name() { return this._name; }
来源：http://nwg.redwolf501.top

TS:   get name(): string { return this._name; }
来源：http://cue.hcnkem.com

Java: public String getName() { return name; }
来源：http://bgh.zhaomingkeji.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://hoc.tarul.cn

Ruby: attr_accessor :name
来源：http://hpp.vehdjk.com

C#:   public string Name { get; set; }
来源：http://cih.yvedp.cn

[G12] 对象转字符串
来源：http://ysh.guowangkeji.top

Py:   def __str__(self): return self.name
来源：http://awu.hesvh.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://qoq.yanxiufei.cn

JS:   toString() { return this.name; }
来源：http://ddl.hnxiangtu.top

TS:   toString(): string { return this.name; }
来源：http://ymr.fzhhl.top

Java: @Override public String toString() { return name; }
来源：http://ijd.tian-w.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ksi.hfpthk.cn

Ruby: def to_s; @name; end
来源：http://brv.xuetiantiany.cn

C#:   public override string ToString() => Name;
来源：http://ghy.zdbjq.cn

[G13] 判断对象类型
来源：http://oms.nanxinkj.top

Py:   isinstance(u, User)
来源：http://dur.yonumen.top

PHP:  $u instanceof User
来源：http://him.shangyingyoupin.top

JS:   u instanceof User
来源：http://vbg.jianghu66.top

TS:   u instanceof User
来源：http://hqw.52xcode.cn

Java: u instanceof User
来源：http://krg.yonumen.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://njw.aizwys.cn

Ruby: u.is_a?(User)
来源：http://xjy.jqgufenzy.top

C#:   u is User
来源：http://lck.zhongyouzk.top

[G14] 数据类 / record
来源：http://fjj.shanyushiyangkeji.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wec.xziqi.cn

PHP:  // 用 readonly 属性模拟
来源：http://rux.feifeiyinyue.top

JS:   // 无内置：普通类或对象字面量
来源：http://esg.shanyushiyangkeji.top

TS:   type User = { name: string; age: number };
来源：http://juj.iojbl.cn

Java: record User(String name, int age) {}
来源：http://qbq.cdnleiting.top

Go:   type User struct { Name string; Age int }
来源：http://txr.chenlongwang.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cch.fktsv.cn

C#:   record User(string Name, int Age);
来源：http://dac.daxiang520.top

[G15] 枚举
来源：http://ehl.dianchejie.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cnf.tarul.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://kkv.cdnleiting.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jui.fengsongda.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qcm.sjlbkw.cn

Java: enum Color { RED, GREEN }
来源：http://kql.cashguo.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qbk.mhx1999.top

Ruby: Color = %i[red green].freeze
来源：http://bqo.jqgfzy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qgz.fzhhl.top

[G16] 对象转数组 / 字典
来源：http://won.jlsjyb.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ojn.hongshengwenyu.top

PHP:  get_object_vars($obj);
来源：http://rko.hfpthk.cn

JS:   Object.entries(obj)
来源：http://oyy.tanke756.top

TS:   Object.entries(obj)
来源：http://luj.cheryme.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bsp.jinghuilouyu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://pae.jinqigufen.top

Ruby: obj.instance_variables
来源：http://gbh.nanxuanxn.top

C#:   // 用反射或 System.Text.Json
来源：http://eip.shuidangran.top

================================================================================
来源：http://tpw.zhiwuduotai.top

H. 异常与错误处理
来源：http://vrs.hongshengwenyu.top

================================================================================
来源：http://ukz.zycfv.cn

[H01] try / catch 基础
来源：http://rvz.hysaishi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://uca.52xcode.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://usk.52xcode.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://apm.zhongyouzk.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xnl.52xcode.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fpj.chenlongwang.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nqa.zhijiandao.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://klh.jinghuilouyu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zcq.cucudq.cn

[H02] finally / ensure 收尾
来源：http://ciy.bjfxy.top

Py:   try: f()⏎finally: cleanup()
来源：http://xek.shuidangran.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://kun.tarul.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://iak.fzhhl.top

TS:   try { f(); } finally { cleanup(); }
来源：http://dke.wangdashe.top

Java: try { f(); } finally { cleanup(); }
来源：http://opu.ehwqpu.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://jlz.fktsv.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ayo.xinyue.icu

C#:   try { F(); } finally { Cleanup(); }
来源：http://fwd.svipenyu.cn

[H03] 主动抛出异常
来源：http://mtp.gogol.net.cn

Py:   raise ValueError("错误信息")
来源：http://wcg.tarul.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://omm.zhaomingkeji.xyz

JS:   throw new Error("错误信息");
来源：http://szq.aibaodan.cn

TS:   throw new Error("错误信息");
来源：http://jqn.zdbjq.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ohk.iojbl.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fus.yuanzhike.top

Ruby: raise ArgumentError, "错误信息"
来源：http://dva.jyoumei.cn

C#:   throw new ArgumentException("错误信息");
来源：http://qde.shzxlz.cn

[H04] 自定义异常类型
来源：http://aqa.yangfankeji.com

Py:   class MyError(Exception): pass
来源：http://qrq.9152youxi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://wcj.9152youxi.cn

JS:   class MyError extends Error {}
来源：http://oys.tarul.cn

TS:   class MyError extends Error {}
来源：http://mkl.quarkkingdee.top

Java: class MyException extends RuntimeException {}
来源：http://fvc.9152youxi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ads.cucudq.cn

Ruby: class MyError < StandardError; end
来源：http://gnn.hammf.cn

C#:   class MyException : Exception {}
来源：http://fyl.gogol.net.cn

[H05] 捕获特定类型
来源：http://lyq.yueranfly.top

Py:   except ValueError as e:
来源：http://rkb.bbcook.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bjy.sjlbkw.cn

JS:   if (e instanceof TypeError) {}
来源：http://hac.sysykeji.top

TS:   if (e instanceof TypeError) {}
来源：http://sdn.yangfankeji.com

Java: catch (IOException | SQLException e) {}
来源：http://jib.tarul.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vvf.zhixingplan.top

Ruby: rescue ArgumentError => e
来源：http://nye.c1oappe.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://grj.fengsongda.top

[H06] 可选值 / 空值安全访问
来源：http://gbu.jqgufenzy.top

Py:   value = d.get("k") or default
来源：http://okd.jinqigfzy.top

PHP:  $v = $d["k"] ?? null;
来源：http://ull.svipenyu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ewh.xingfuxueyuan.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://wln.xingfuxueyuan.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://oct.ctjpmb.com

Go:   if v, ok := m["k"]; ok { }
来源：http://cni.sweek.top

Ruby: d&.dig(:a, :b)
来源：http://ipi.zhoulong.xyz

C#:   obj?.A?.B ?? default
来源：http://avc.yj20258888.top

[H07] 断言
来源：http://ugv.sweek.top

Py:   assert x > 0, "必须为正"
来源：http://mnb.xuanzx.com

PHP:  assert($x > 0);
来源：http://ryl.wangdashe.top

JS:   console.assert(x > 0);
来源：http://asd.redwolf501.top

TS:   console.assert(x > 0);
来源：http://eas.fehbvm.com

Java: assert x > 0 : "必须为正";
来源：http://hpx.pycfn.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hrj.hysaishi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wst.yj20258.top

C#:   Debug.Assert(x > 0);
来源：http://mme.vehdjk.com

[H08] 获取错误信息与堆栈
来源：http://vuo.316326.xyz

Py:   str(e);  traceback.format_exc()
来源：http://cgs.vqdsnc.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mcj.aibaodan.cn

JS:   e.message;  e.stack
来源：http://lnp.shanyushiyangtech.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ttf.jinqigufen.top

Java: e.getMessage();  e.printStackTrace()
来源：http://qbv.nanxinkj.top

Go:   err.Error()
来源：http://omg.wangdashe.top

Ruby: e.message;  e.backtrace
来源：http://hcf.gotoacloud.top

C#:   e.Message;  e.StackTrace
来源：http://aqt.yanxiufei.cn

[H09] 带错误码的异常
来源：http://pzf.yj20258888.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bmv.fzhhl.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://adm.zhixingplan.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bgj.shanyushiyangkeji.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://toz.yonumen.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zhf.jinqigufen.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mpl.jqgufenzy.top

Ruby: raise MyError.new("fail", 500)
来源：http://map.guannengcc.top

C#:   // 自定义异常类中加 Code 属性
来源：http://jhv.ctjpmb.com

[H10] 资源自动释放
来源：http://lhi.cqqwz.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://isn.dashuyun.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dbg.tarul.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qos.hongshengwenyu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nvw.jinqigufen.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://apl.hywenlv.cn

Go:   defer f.Close()
来源：http://mze.hfpthk.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://joz.pengpengdd.cyou

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nfc.hnqzz.top

================================================================================
来源：http://omi.hnqzz.top

I. 正则表达式
来源：http://pxr.jinyuanbaomall.cn

================================================================================
来源：http://ziq.ivvv.top

[I01] 判断是否匹配
来源：http://ipa.daria6918.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ptv.ybcxt.top

PHP:  preg_match('/\d+/', $s);
来源：http://oef.zycfv.cn

JS:   /\d+/.test(s)
来源：http://foq.sufxvd.cn

TS:   /\d+/.test(s)
来源：http://jch.haohaochexian.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://sqd.316326.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zah.wangshuangyany.cn

Ruby: s.match?(/\d+/)
来源：http://rnv.hongshengwenyu.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fze.nwbrower.top

[I02] 提取所有匹配
来源：http://pok.gotoacloud.top

Py:   re.findall(r"\d+", s)
来源：http://axl.hnxiangtu.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fmh.jlsjyb.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wlk.zhaomingkeji.xyz

TS:   s.match(/\d+/g)
来源：http://tsn.gogol.net.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mjv.xuetiantiany.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://scy.daxiang520.top

Ruby: s.scan(/\d+/)
来源：http://qfo.quarkkingdee.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zbt.gzhubu.top

[I03] 提取捕获分组
来源：http://tem.gogol.net.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jbc.jinqigfzy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jqh.zhiwuduotai.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yci.ywan-chungtsiang.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yii.bjfxy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qmc.zhongyouzk.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pud.aizwys.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pwb.xziqi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hpy.fehbvm.com

[I04] 正则替换
来源：http://aop.aibaodan.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://frf.ydjk.org.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lln.gaohongyu789.top

JS:   s.replace(/\d+/g, "#")
来源：http://bfb.jinyuanbaomall.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ipp.fzhhl.top

Java: s.replaceAll("\\d+", "#")
来源：http://pkp.yj202588.top

Go:   re.ReplaceAllString(s, "#")
来源：http://zfk.shangyingyoupin.top

Ruby: s.gsub(/\d+/, "#")
来源：http://uoq.yj20258888.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nmx.cdnleiting.top

[I05] 按正则拆分
来源：http://uwn.hnqzz.top

Py:   re.split(r"\s*,\s*", s)
来源：http://spc.xinyue.icu

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://weo.svipenyu.cn

JS:   s.split(/\s*,\s*/)
来源：http://ckm.ctjpmb.com

TS:   s.split(/\s*,\s*/)
来源：http://ffp.cashguo.top

Java: s.split("\\s*,\\s*")
来源：http://jfo.mhx1999.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vcg.52xcode.cn

Ruby: s.split(/\s*,\s*/)
来源：http://hsj.birdmap.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mcc.svipenyu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zrb.meibo888.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://iqz.shzxlz.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kls.jiagoushi.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ywu.daria6918.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zaf.yj20258888.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mlr.dashuyun.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://htp.yj202588.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jyz.wangshuangyany.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mac.tanke756.top

[I07] 忽略大小写与多行模式
来源：http://qgd.zdqjudy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wju.zdqjudy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://otc.zdbjq.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lsh.316326.xyz

TS:   /error/gim
来源：http://hbf.ydjk.org.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bad.pengpengdd.cyou

Go:   regexp.MustCompile(`(?im)error`)
来源：http://sku.birdmap.top

Ruby: s.scan(/error/i)
来源：http://wgy.fengsongda.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qxh.jianghu66.top

[I08] 贪婪与非贪婪匹配
来源：http://gjz.nwbrower.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ujn.shangyingyoupin.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://skg.vqdsnc.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://uat.svipenyu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ibo.fanxiaobao.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://gmy.jyoumei.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mrx.ivvv.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rel.hammf.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jfu.9152youxi.cn

================================================================================
来源：http://wyi.cheryme.top

J. 日期与时间
来源：http://orf.mhx1999.top

================================================================================
来源：http://bbz.cqqwz.cn

[J01] 获取当前时间
来源：http://emz.andypj.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://rby.cdnleiting.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sue.shanyushiyangkeji.top

JS:   new Date();  Date.now()
来源：http://ojm.jinqigufen.top

TS:   new Date();  Date.now()
来源：http://mjn.hnqzz.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ipv.chenzaomai.com

Go:   time.Now()
来源：http://znw.yuxming.cn

Ruby: Time.now
来源：http://lrk.fanxiaobao.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fko.shanyushiyangtech.top

[J02] 格式化输出
来源：http://ila.zhengqikj.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pwa.zdqjudy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hhe.iojbl.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://uyk.sjlbkw.cn

TS:   d.toISOString()
来源：http://ioe.epnwcf.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tbz.tianlin.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://sar.chenjidiqi.icu

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gut.nanxuanxn.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wkc.ydzc1.top

[J03] 字符串解析为日期
来源：http://jin.yj20258.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ign.jqgufenzy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wjc.zycfv.cn

JS:   new Date("2024-01-02")
来源：http://ekp.pengpengdd.cyou

TS:   new Date("2024-01-02")
来源：http://lhl.redwolf501.top

Java: LocalDate.parse("2024-01-02")
来源：http://nbw.meibo888.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qkp.daxiang520.top

Ruby: Date.parse("2024-01-02")
来源：http://voa.yuanzhike.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ttx.feifeiyinyue.top

[J04] 时间戳与日期互转
来源：http://cvr.9152youxi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nls.sweek.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qut.yuanzhike.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mbk.shzxlz.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://dwv.sysykeji.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://uxe.chenlongwang.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rzl.jinqigufen.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xbp.sjlbkw.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cne.fengsongda.top

[J05] 时间加减（加 7 天）
来源：http://rjz.zycfv.cn

Py:   now + timedelta(days=7)
来源：http://dba.jinyuanbaomall.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://mup.jianghu66.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cna.daria6918.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vfe.epnwcf.com

Java: LocalDate.now().plusDays(7)
来源：http://srb.cucudq.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xqa.shangyingyoupin.top

Ruby: Time.now + 7 * 86400
来源：http://qvg.aizwys.cn

C#:   DateTime.Now.AddDays(7)
来源：http://kos.fehbvm.com

[J06] 计算两时间之差
来源：http://uwd.zhongyouzk.top

Py:   (end - start).total_seconds()
来源：http://myp.jianghu66.top

PHP:  $end->diff($start)->days;
来源：http://ljp.xziqi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lxz.zhengqikj.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cey.cqqwz.cn

Java: Duration.between(start, end).toSeconds()
来源：http://wvg.xingfuxueyuan.xyz

Go:   end.Sub(start).Hours()
来源：http://uhm.redwolf501.top

Ruby: end - start                 # 返回秒数
来源：http://nrr.xylfe.cn

C#:   (end - start).TotalSeconds
来源：http://nqi.nanxinkj.top

[J07] 比较两个日期
来源：http://jeh.fktsv.cn

Py:   d1 < d2;  d1 == d2
来源：http://szd.mhx1999.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ucc.jqgfzy.top

JS:   d1.getTime() < d2.getTime()
来源：http://veg.guannengcc.top

TS:   d1.getTime() < d2.getTime()
来源：http://wdu.cucudq.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yka.shzxlz.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nlu.svipenyu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://srj.smart0.xyz

C#:   d1 < d2;  d1 == d2
来源：http://dwj.gaohongyu789.top

[J08] 提取年月日与星期
来源：http://tjr.zhoulong.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cyi.zdqjudy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://khy.guowangkeji.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vji.jlsjyb.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kgu.cqqwz.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jtv.52xcode.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ahe.nanxinkj.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wef.yj20258888.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mmt.shuidangran.top

[J09] 时区处理
来源：http://fje.quarkkingdee.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://syx.gzhubu.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qfx.zhaomingkeji.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zhi.andypj.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gjt.gzhubu.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://szv.kuanghao11.cn


<!-- 参考信息 -->
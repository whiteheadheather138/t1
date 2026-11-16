代发 wailian999

[Q76] 按天统计
来源：http://nyy.hcnkem.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fhy.fengsongda.top

[Q77] 时间加减
来源：http://mqy.tanke756.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pei.pengpengdd.cyou

[Q78] 当前时间
来源：http://jpo.fengsongda.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kiz.cdnleiting.top

[Q79] 字符串拼接
来源：http://wdo.quarkkingdee.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gro.ehwqpu.com

[Q80] 字符串截取
来源：http://kfs.xuanzx.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://uhq.redwolf501.top

[Q81] 字符串替换
来源：http://sil.bbcook.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zip.shangyingyoupin.top

[Q82] 字符长度与字节长度
来源：http://zib.jianghu66.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qmi.zdqjudy.top

[Q83] 大小写转换
来源：http://tdj.fengsongda.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dys.yonumen.top

[Q84] 去除首尾空格
来源：http://ivg.wangdashe.top

SELECT TRIM(name) FROM users;
来源：http://kzf.shangyingyoupin.top

[Q85] 数值取整
来源：http://ity.jinyuanbaomall.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tjw.pengpengdd.cyou

[Q86] 读取 JSON 字段
来源：http://ohb.aizwys.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vdn.yj20258888.top

[Q87] JSON 字段做条件
来源：http://qtq.cdnleiting.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rxq.yj20258.top

[Q88] 行转列（条件聚合）
来源：http://pvq.pycfn.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://udz.wangshuangyany.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jte.ppjwa.cn

[Q89] 判断表是否存在
来源：http://yrh.chenzaomai.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://btx.pycfn.com

[Q90] 生成序号列
来源：http://ksf.tianlin.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tus.yangfankeji.com

================================================================================
来源：http://kpf.andypj.xyz

R. Bash 专题
来源：http://sjh.ehwqpu.com

================================================================================
来源：http://uyt.tanke756.top

[R01] shebang 与严格模式
来源：http://kgd.sjlbkw.cn

#!/usr/bin/env bash
来源：http://lrn.cqqwz.cn

set -euo pipefail
来源：http://lgu.52xcode.cn

[R02] 变量赋值与使用
来源：http://knl.tanke756.top

name="Tom"; echo "$name"
来源：http://urq.0kj1m.cn

[R03] 只读变量
来源：http://nsl.vehdjk.com

readonly PI=3.14
来源：http://rzb.jqgfzy.top

[R04] 位置参数
来源：http://ijt.epnwcf.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jll.hcnkem.com

[R05] 参数默认值
来源：http://jqk.jinyuanbaomall.cn

name="${1:-default}"
来源：http://aqf.zhijiandao.cn

[R06] 判断命令是否存在
来源：http://hes.svipenyu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uad.wangshuangyany.cn

[R07] if 判断文件
来源：http://xih.fengsongda.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xas.uphjek.com

[R08] 数值比较
来源：http://smj.yongpay.top

if (( a > b )); then echo "a 更大"; fi
来源：http://med.daria6918.cn

[R09] 字符串比较
来源：http://urx.vqdsnc.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cqn.dashuyun.cn

[R10] 正则匹配
来源：http://ikw.hcnkem.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ozr.cucudq.cn

[R11] case 多分支
来源：http://tyx.nanxuanxn.top

case "$1" in
来源：http://zrh.yfazqb.com

start) echo "启动" ;;
来源：http://pev.shangyingyoupin.top

stop)  echo "停止" ;;
来源：http://pmx.jqgufenzy.top

*)     echo "未知命令" ;;
来源：http://utf.jlsjyb.cn

esac
来源：http://ykr.jyoumei.cn

[R12] for 遍历文件
来源：http://hfv.hfpthk.cn

for f in *.txt; do echo "$f"; done
来源：http://nua.yj20258888.top

[R13] for 计数循环
来源：http://lwr.hnqzz.top

for i in {1..10}; do echo "$i"; done
来源：http://kkd.0kj1m.cn

[R14] C 风格 for
来源：http://jlz.mhx1999.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lud.nwbrower.top

[R15] while 逐行读文件
来源：http://zic.daxiang520.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kge.jinyuanbaomall.cn

[R16] until 等待条件
来源：http://ahe.zhiwuduotai.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ocm.ehwqpu.com

[R17] 数组定义与取值
来源：http://hfp.shanyushiyangkeji.top

arr=(a b c); echo "${arr[0]}"
来源：http://nig.yueranfly.top

[R18] 遍历数组
来源：http://ygr.jianghu66.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://adt.zhaomingkeji.xyz

[R19] 数组长度
来源：http://clj.zdbjq.cn

echo "${#arr[@]}"
来源：http://qlf.fktsv.cn

[R20] 关联数组（字典）
来源：http://aff.yueranfly.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gam.gogol.net.cn

[R21] 字符串长度
来源：http://qim.ydzc1.top

echo "${#s}"
来源：http://haa.smart0.xyz

[R22] 截取子串
来源：http://uyg.chenlongwang.top

echo "${s:0:5}"
来源：http://knd.yanxiufei.cn

[R23] 字符串替换
来源：http://sod.jqgufenzy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nie.cqqwz.cn

[R24] 大小写转换
来源：http://qwa.guowangkeji.top

echo "${s^^}"; echo "${s,,}"
来源：http://kws.yj202588.top

[R25] 去后缀 / 去前缀
来源：http://xbk.nanxinkj.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://lae.zhongyouzk.top

[R26] 命令替换
来源：http://qii.gogol.net.cn

now=$(date +%F); echo "$now"
来源：http://bxa.xingfuxueyuan.xyz

[R27] 算术展开
来源：http://onv.tianlin.xyz

echo $((1 + 2 * 3))
来源：http://ifw.gogol.net.cn

[R28] 浮点运算
来源：http://ehp.zdbjq.cn

echo "scale=2; 10/3" | bc
来源：http://hcx.fehbvm.com

[R29] 定义函数
来源：http://hqg.snrcjt.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ahq.yongpay.top

[R30] 函数返回状态码
来源：http://srt.gzhubu.top

f() { return 0; }; f || echo "失败了"
来源：http://ozk.ctjpmb.com

[R31] 局部变量
来源：http://uta.cqqwz.cn

f() { local x=1; echo "$x"; }
来源：http://gek.fktsv.cn

[R32] 参数个数校验
来源：http://ybi.daxiang520.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zry.jiagoushi.top

[R33] 捕获错误并提示行号
来源：http://awd.ydjk.org.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kmu.yuanzhike.top

[R34] 退出时清理
来源：http://tkz.uphjek.com

trap 'rm -f "$tmp"' EXIT
来源：http://kdx.shzxlz.cn

[R35] 后台执行并等待
来源：http://ldr.fanxiaobao.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://wpt.yanxiufei.cn

[R36] 并发执行多个任务
来源：http://fjc.yangfankeji.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vgy.xingfuxueyuan.xyz

[R37] 把输出赋给变量
来源：http://afw.guowangkeji.top

files=$(ls -1)
来源：http://oqx.zhongyouzk.top

[R38] 管道串联
来源：http://tds.gzhubu.top

cat a.txt | grep -i error | wc -l
来源：http://uqk.smart0.xyz

[R39] 重定向标准输出与错误
来源：http://cqk.birdmap.top

cmd > out.log 2>&1
来源：http://mia.sysykeji.top

[R40] 追加写日志
来源：http://wws.zhengqikj.top

echo "log" >> out.log
来源：http://gxx.shuidangran.top

[R41] 丢弃输出
来源：http://ypc.yj20258.top

cmd >/dev/null 2>&1
来源：http://uev.xingfuxueyuan.xyz

[R42] 输入重定向
来源：http://dmx.fengsongda.top

wc -l < a.txt
来源：http://zcg.bjfxy.top

[R43] 按名字查找文件
来源：http://qzl.xziqi.cn

find . -name "*.log" -type f
来源：http://flz.vehdjk.com

[R44] 按修改时间查找
来源：http://cqm.chenlongwang.top

find . -mtime -7 -type f
来源：http://wvl.c1oappe.top

[R45] 批量删除
来源：http://gxy.nwbrower.top

find . -name "*.tmp" -delete
来源：http://hnb.jqgfzy.top

[R46] 递归替换文件内容
来源：http://lin.ehwqpu.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vkg.xingfuxueyuan.xyz

[R47] sed 单行替换
来源：http://aem.cheryme.top

sed -i 's/foo/bar/g' a.txt
来源：http://ezb.birdmap.top

[R48] awk 取指定列
来源：http://nog.daxiang520.top

awk '{print $1, $3}' a.txt
来源：http://dfz.xinyue.icu

[R49] awk 带条件
来源：http://hmq.sweek.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ghw.jinqigfzy.top

[R50] awk 求和
来源：http://orr.jianghu66.top

awk '{s += $2} END {print s}' a.txt
来源：http://czf.pycfn.com

[R51] 排序去重取前几
来源：http://mvb.jinqigfzy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://skh.gogol.net.cn

[R52] 统计行数
来源：http://sro.aibaodan.cn

wc -l a.txt
来源：http://wow.xylfe.cn

[R53] 查看文件头与实时尾
来源：http://yzx.ehwqpu.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gri.sweek.top

[R54] 比较两个文件
来源：http://ipu.sweek.top

diff a.txt b.txt
来源：http://bhm.daria6918.cn

[R55] 压缩与解压
来源：http://gyj.cqqwz.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vnn.jqgfzy.top

[R56] 远程拷贝
来源：http://svc.tarul.cn

scp file user@host:/path/
来源：http://ulq.sweek.top

[R57] 远程执行命令
来源：http://xqi.chenzaomai.com

ssh user@host 'uptime'
来源：http://yxu.aizwys.cn

[R58] 下载文件
来源：http://gvf.yangfankeji.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tja.316326.xyz

[R59] 发 POST JSON
来源：http://qhv.jinqigufen.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nkz.nanxinkj.top

[R60] 只看 HTTP 状态码
来源：http://alq.vqdsnc.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://boj.feifeiyinyue.top

[R61] 磁盘占用
来源：http://dzt.c1oappe.top

df -h;  du -sh *
来源：http://uez.fehbvm.com

[R62] 找最占空间的文件
来源：http://ufp.hnqzz.top

du -ah . | sort -rh | head -10
来源：http://rmt.fzhhl.top

[R63] 内存与进程
来源：http://ssq.jinqigufen.top

free -h;  ps aux | grep nginx
来源：http://prf.hnqzz.top

[R64] 结束进程
来源：http://npe.xylfe.cn

kill -9 $(pgrep -f app.py)
来源：http://yln.aibaodan.cn

[R65] 查看端口占用
来源：http://xjk.haohaochexian.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xgb.mhx1999.top

[R66] 定时任务
来源：http://wdf.pycfn.com

crontab -e;  crontab -l
来源：http://wkj.xinyue.icu

[R67] 生成随机十六进制串
来源：http://zcj.hysaishi.cn

openssl rand -hex 16
来源：http://ogr.iojbl.cn

[R68] 计算文件校验值
来源：http://nek.sufxvd.cn

sha256sum a.txt;  md5sum a.txt
来源：http://hoc.jinqigfzy.top

[R69] 生成随机密码
来源：http://rsx.chenzaomai.com

head -c 16 /dev/urandom | base64
来源：http://ays.jqgufenzy.top

[R70] 时间戳与互转
来源：http://mbi.tarul.cn

date +%s;  date -d @1700000000
来源：http://lxl.wangdashe.top

[R71] 日期格式化
来源：http://mrc.jinghuilouyu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://yxd.fktsv.cn

[R72] 等待端口就绪
来源：http://vpd.zhiwuduotai.top

until nc -z localhost 3306; do sleep 1; done
来源：http://don.fehbvm.com

[R73] 分割大日志
来源：http://rpg.hysaishi.cn

split -l 1000 big.log part_
来源：http://lwl.hnxiangtu.top

[R74] 批量重命名
来源：http://oux.yangfankeji.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gih.redwolf501.top

[R75] 导出环境变量
来源：http://rpj.hnxiangtu.top

export PATH="$HOME/bin:$PATH"
来源：http://fmt.havefunace.top

[R76] 使用临时文件
来源：http://dub.cashguo.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lht.tianlin.xyz

[R77] 读取用户输入
来源：http://pfq.shangyingyoupin.top

read -rp "请输入: " ans
来源：http://beo.vqdsnc.cn

[R78] 交互式菜单
来源：http://uyn.yongpay.top

select opt in a b c; do echo "$opt"; break; done
来源：http://moa.feifeiyinyue.top

[R79] 解析命令行选项
来源：http://xzx.jinqigfzy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://frr.ywan-chungtsiang.top

[R80] 查看脚本执行耗时
来源：http://szs.cucudq.cn

time ./run.sh
来源：http://ttj.yanxiufei.cn

================================================================================
来源：http://vxc.havefunace.top

S. C / C++ 专题
来源：http://xib.xinyue.icu

================================================================================
来源：http://vbx.aizwys.cn

[S01] C：Hello World
来源：http://ajb.zhaomingkeji.xyz

#include <stdio.h>
来源：http://zek.svipenyu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://afh.iojbl.cn

[S02] C：变量与格式化输出
来源：http://pcv.jinghuilouyu.cn

int a = 10; printf("%d\n", a);
来源：http://flj.guannengcc.top

[S03] C：读入整数
来源：http://svl.chenlongwang.top

int x; scanf("%d", &x);
来源：http://jdb.cucudq.cn

[S04] C：字符串复制
来源：http://czp.hongshengwenyu.top

char dst[32]; strcpy(dst, "hi");
来源：http://lay.cucudq.cn

[S05] C：字符串长度
来源：http://lxf.nwbrower.top

strlen(s)
来源：http://jpo.dianchejie.cn

[S06] C：字符串比较
来源：http://xvy.316326.xyz

strcmp(a, b) == 0
来源：http://flk.ydjk.org.cn

[S07] C：数组遍历求和
来源：http://daq.ppjwa.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qkb.yj20258.top

[S08] C：动态内存分配与释放
来源：http://yrn.xinyue.icu

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bbn.zhixingplan.top

[S09] C：结构体定义与初始化
来源：http://qkg.nwbrower.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ual.jinyuanbaomall.cn

[S10] C：指针与解引用
来源：http://whw.snrcjt.cn

int *p = &a;  *p = 5;
来源：http://mwd.zhixingplan.top

[S11] C：逐行读文件
来源：http://aak.dianchejie.cn

FILE *f = fopen("a.txt", "r");
来源：http://yid.sjlbkw.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xim.cheryme.top

fclose(f);
来源：http://odg.hnxiangtu.top

[S12] C：写文件
来源：http://xtr.sweek.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tcl.cucudq.cn

[S13] C：宏定义
来源：http://tbu.gogol.net.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lyr.fehbvm.com

[S14] C：枚举
来源：http://gvy.hnqzz.top

enum Color { RED, GREEN, BLUE };
来源：http://fps.sjlbkw.cn

[S15] C：类型转换
来源：http://jrm.zdqjudy.top

(double) a / b
来源：http://kqe.yueranfly.top

[S16] C：位操作置位
来源：http://zrc.pycfn.com

x |= (1 << 3);
来源：http://oiw.yanxiufei.cn

[S17] C：安全拼接字符串
来源：http://vhf.sweek.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rea.xziqi.cn

[S18] C：命令行参数
来源：http://jwv.redwolf501.top

int main(int argc, char **argv)
来源：http://jvx.yongpay.top

[S19] C：快速排序
来源：http://dsb.316326.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://qch.andypj.xyz

[S20] C：二分查找
来源：http://eat.fzhhl.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://oon.xingfuxueyuan.xyz

[S21] C：字符类别判断
来源：http://drw.quarkkingdee.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dsv.9152youxi.cn

[S22] C：字符串转数字
来源：http://xfc.yj20258.top

atoi("42");  strtod("3.14", NULL);
来源：http://kjj.snrcjt.cn

[S23] C：随机数
来源：http://cga.ppjwa.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://nam.gzhubu.top

[S24] C：获取本地时间
来源：http://vln.wangdashe.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://drk.sysykeji.top

[S25] C：内存拷贝
来源：http://bwc.tian-w.cn

memcpy(dst, src, n);
来源：http://jqt.ydzc1.top

[S26] C：内存清零
来源：http://jft.bjfxy.top

memset(a, 0, sizeof a);
来源：http://gql.jqgfzy.top

[S27] C：定义常量
来源：http://hac.dashuyun.cn

const double PI = 3.14159;
来源：http://mdd.gogol.net.cn

[S28] C：静态变量
来源：http://prk.cashguo.top

static int counter = 0;
来源：http://fxg.shanyushiyangkeji.top

[S29] C：变参函数
来源：http://ocu.yuxming.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wjf.yuanzhike.top

[S30] C：头文件保护
来源：http://ivc.fehbvm.com

#ifndef X_H
来源：http://syn.bjfxy.top

#define X_H
来源：http://xrf.jyoumei.cn

#endif
来源：http://dmp.shangyingyoupin.top

[S31] C++：Hello World
来源：http://rtl.mhx1999.top

#include <iostream>
来源：http://fap.guannengcc.top

int main() { std::cout << "Hello\n"; }
来源：http://tnu.yonumen.top

[S32] C++：字符串
来源：http://cag.chenjidiqi.icu

std::string s = "hi";  s += "!";
来源：http://zrv.kuanghao11.cn

[S33] C++：vector 增删
来源：http://njo.tian-w.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wln.yj20258.top

[S34] C++：遍历 vector
来源：http://zub.xylfe.cn

for (auto &x : v) { std::cout << x; }
来源：http://hnl.gzhubu.top

[S35] C++：map
来源：http://zhf.jianghu66.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://whf.sweek.top

[S36] C++：unordered_map
来源：http://rmi.yj20258.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://szf.fengsongda.top

[S37] C++：set
来源：http://nms.ivvv.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://end.ydzc1.top

[S38] C++：排序
来源：http://yek.cqqwz.cn

std::sort(v.begin(), v.end());
来源：http://fvf.jinyuanbaomall.cn

[S39] C++：自定义比较器排序
来源：http://jay.guannengcc.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bcg.gotoacloud.top

[S40] C++：查找元素
来源：http://dnw.hywenlv.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ztv.tian-w.cn

[S41] C++：类与构造函数
来源：http://ydt.xuetiantiany.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://izv.ydzc1.top

[S42] C++：继承与虚函数
来源：http://vmf.52xcode.cn

class B : public Base { public: void f() override {} };
来源：http://qtt.bjfxy.top

[S43] C++：智能指针
来源：http://kln.jqgfzy.top

auto p = std::make_unique<int>(5);
来源：http://hlr.gzhubu.top

[S44] C++：引用传参
来源：http://ovs.zhixingplan.top

void inc(int &x) { ++x; }
来源：http://pzg.aibaodan.cn

[S45] C++：lambda
来源：http://gnb.gotoacloud.top

auto add = [](int a, int b) { return a + b; };
来源：http://gie.yueranfly.top

[S46] C++：函数模板
来源：http://qdp.yj20258888.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yeo.shanyushiyangtech.top


<!-- 参考信息 -->
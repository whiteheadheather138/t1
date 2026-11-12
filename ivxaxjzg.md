代发 wailian999

[Q76] 按天统计
来源：http://khb.yj202588.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://leh.hongshengwenyu.top

[Q77] 时间加减
来源：http://tjk.havefunace.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tim.zycfv.cn

[Q78] 当前时间
来源：http://jwd.tanke756.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://iye.bbcook.cn

[Q79] 字符串拼接
来源：http://com.nanxuanxn.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ocq.sxryk.cn

[Q80] 字符串截取
来源：http://gyi.yj20258888.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://soj.vqdsnc.cn

[Q81] 字符串替换
来源：http://bsb.chenjidiqi.icu

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ldj.feifeiyinyue.top

[Q82] 字符长度与字节长度
来源：http://adk.cheryme.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://asf.yuanzhike.top

[Q83] 大小写转换
来源：http://tqj.hnxiangtu.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qay.daria6918.cn

[Q84] 去除首尾空格
来源：http://qft.yangfankeji.com

SELECT TRIM(name) FROM users;
来源：http://vvi.wangshuangyany.cn

[Q85] 数值取整
来源：http://tai.316326.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://osa.shangyingyoupin.top

[Q86] 读取 JSON 字段
来源：http://plf.gotoacloud.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pdx.kuanghao11.cn

[Q87] JSON 字段做条件
来源：http://mua.hysaishi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hav.sysykeji.top

[Q88] 行转列（条件聚合）
来源：http://dwf.vehdjk.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jne.guowangkeji.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cic.redwolf501.top

[Q89] 判断表是否存在
来源：http://ttl.tianlin.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tca.feifeiyinyue.top

[Q90] 生成序号列
来源：http://usf.0kj1m.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dwm.zhixingplan.top

================================================================================
来源：http://dzr.bbcook.cn

R. Bash 专题
来源：http://ifd.chenzaomai.com

================================================================================
来源：http://axt.gaohongyu789.top

[R01] shebang 与严格模式
来源：http://rmi.xinyue.icu

#!/usr/bin/env bash
来源：http://cfp.nanxuanxn.top

set -euo pipefail
来源：http://toq.shuidangran.top

[R02] 变量赋值与使用
来源：http://qwl.fzhhl.top

name="Tom"; echo "$name"
来源：http://qys.fktsv.cn

[R03] 只读变量
来源：http://ylt.pengpengdd.cyou

readonly PI=3.14
来源：http://otn.cqqwz.cn

[R04] 位置参数
来源：http://tqo.fanxiaobao.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ecw.zdqjudy.top

[R05] 参数默认值
来源：http://amj.sweek.top

name="${1:-default}"
来源：http://uur.vehdjk.com

[R06] 判断命令是否存在
来源：http://eld.andypj.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ypl.feifeiyinyue.top

[R07] if 判断文件
来源：http://drn.shuidangran.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xgg.jqgufenzy.top

[R08] 数值比较
来源：http://huo.jinghuilouyu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://vxd.tian-w.cn

[R09] 字符串比较
来源：http://ose.zhixingplan.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rzd.shanyushiyangtech.top

[R10] 正则匹配
来源：http://due.yanxiufei.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wqg.sysykeji.top

[R11] case 多分支
来源：http://ktn.shzxlz.cn

case "$1" in
来源：http://gez.birdmap.top

start) echo "启动" ;;
来源：http://yop.0kj1m.cn

stop)  echo "停止" ;;
来源：http://bki.yuanzhike.top

*)     echo "未知命令" ;;
来源：http://nzb.jlsjyb.cn

esac
来源：http://zhu.9152youxi.cn

[R12] for 遍历文件
来源：http://jwb.zdbjq.cn

for f in *.txt; do echo "$f"; done
来源：http://efw.chenjidiqi.icu

[R13] for 计数循环
来源：http://oog.xingfuxueyuan.xyz

for i in {1..10}; do echo "$i"; done
来源：http://dsg.ydzc1.top

[R14] C 风格 for
来源：http://nra.zdqjudy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yky.zhoulong.xyz

[R15] while 逐行读文件
来源：http://gaf.yangfankeji.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://aqx.redwolf501.top

[R16] until 等待条件
来源：http://iyo.jiagoushi.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hmq.gotoacloud.top

[R17] 数组定义与取值
来源：http://qbo.aizwys.cn

arr=(a b c); echo "${arr[0]}"
来源：http://bfb.xuetiantiany.cn

[R18] 遍历数组
来源：http://ffl.smart0.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://aqh.shanyushiyangkeji.top

[R19] 数组长度
来源：http://xzg.hnqzz.top

echo "${#arr[@]}"
来源：http://lxu.ywan-chungtsiang.top

[R20] 关联数组（字典）
来源：http://tjn.ctjpmb.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://atx.mhx1999.top

[R21] 字符串长度
来源：http://fto.xziqi.cn

echo "${#s}"
来源：http://zrv.hysaishi.cn

[R22] 截取子串
来源：http://ohe.zhixingplan.top

echo "${s:0:5}"
来源：http://ucd.zhiwuduotai.top

[R23] 字符串替换
来源：http://goh.quarkkingdee.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cml.dianchejie.cn

[R24] 大小写转换
来源：http://xav.zhongyouzk.top

echo "${s^^}"; echo "${s,,}"
来源：http://ffe.bjfxy.top

[R25] 去后缀 / 去前缀
来源：http://dba.nanxinkj.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ffu.feifeiyinyue.top

[R26] 命令替换
来源：http://auk.yfazqb.com

now=$(date +%F); echo "$now"
来源：http://uvp.feifeiyinyue.top

[R27] 算术展开
来源：http://qxf.jinghuilouyu.cn

echo $((1 + 2 * 3))
来源：http://ipr.jyoumei.cn

[R28] 浮点运算
来源：http://shd.sjlbkw.cn

echo "scale=2; 10/3" | bc
来源：http://vow.yanxiufei.cn

[R29] 定义函数
来源：http://ihp.jqgfzy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://uud.jinghuilouyu.cn

[R30] 函数返回状态码
来源：http://czp.gaohongyu789.top

f() { return 0; }; f || echo "失败了"
来源：http://kvb.chenjidiqi.icu

[R31] 局部变量
来源：http://vit.hfpthk.cn

f() { local x=1; echo "$x"; }
来源：http://whe.fengsongda.top

[R32] 参数个数校验
来源：http://rzf.ybcxt.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cgo.jinqigufen.top

[R33] 捕获错误并提示行号
来源：http://pob.yonumen.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hqc.cheryme.top

[R34] 退出时清理
来源：http://xnq.jyoumei.cn

trap 'rm -f "$tmp"' EXIT
来源：http://luw.wangshuangyany.cn

[R35] 后台执行并等待
来源：http://cmc.cqqwz.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://iyt.jiagoushi.top

[R36] 并发执行多个任务
来源：http://kjn.jyoumei.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qdr.sxryk.cn

[R37] 把输出赋给变量
来源：http://lun.xuanzx.com

files=$(ls -1)
来源：http://wjt.uphjek.com

[R38] 管道串联
来源：http://uip.shzxlz.cn

cat a.txt | grep -i error | wc -l
来源：http://vlp.bjfxy.top

[R39] 重定向标准输出与错误
来源：http://zuv.hnqzz.top

cmd > out.log 2>&1
来源：http://pht.snrcjt.cn

[R40] 追加写日志
来源：http://xvs.cashguo.top

echo "log" >> out.log
来源：http://hzj.gaohongyu789.top

[R41] 丢弃输出
来源：http://asw.xingfuxueyuan.xyz

cmd >/dev/null 2>&1
来源：http://sin.yj20258.top

[R42] 输入重定向
来源：http://wje.xylfe.cn

wc -l < a.txt
来源：http://enl.chenzaomai.com

[R43] 按名字查找文件
来源：http://sxa.9152youxi.cn

find . -name "*.log" -type f
来源：http://ntc.sweek.top

[R44] 按修改时间查找
来源：http://wda.redwolf501.top

find . -mtime -7 -type f
来源：http://chi.snrcjt.cn

[R45] 批量删除
来源：http://bfd.yangfankeji.com

find . -name "*.tmp" -delete
来源：http://aua.ywan-chungtsiang.top

[R46] 递归替换文件内容
来源：http://ecv.zhiwuduotai.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wqn.c1oappe.top

[R47] sed 单行替换
来源：http://mfz.zhongyouzk.top

sed -i 's/foo/bar/g' a.txt
来源：http://tze.dianchejie.cn

[R48] awk 取指定列
来源：http://lkt.yanxiufei.cn

awk '{print $1, $3}' a.txt
来源：http://xek.zdbjq.cn

[R49] awk 带条件
来源：http://dly.hywenlv.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sdo.ywan-chungtsiang.top

[R50] awk 求和
来源：http://gll.guowangkeji.top

awk '{s += $2} END {print s}' a.txt
来源：http://iiy.hnxiangtu.top

[R51] 排序去重取前几
来源：http://uvl.gogol.net.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://osb.jinghuilouyu.cn

[R52] 统计行数
来源：http://yhw.ctjpmb.com

wc -l a.txt
来源：http://wqx.tian-w.cn

[R53] 查看文件头与实时尾
来源：http://cec.xuanzx.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wsv.daxiang520.top

[R54] 比较两个文件
来源：http://lvu.sysykeji.top

diff a.txt b.txt
来源：http://cah.yj202588.top

[R55] 压缩与解压
来源：http://iyx.pycfn.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ghr.hnqzz.top

[R56] 远程拷贝
来源：http://rxa.pycfn.com

scp file user@host:/path/
来源：http://glo.yj202588.top

[R57] 远程执行命令
来源：http://ovo.xuanzx.com

ssh user@host 'uptime'
来源：http://eav.jinghuilouyu.cn

[R58] 下载文件
来源：http://bau.ctjpmb.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://uic.gaohongyu789.top

[R59] 发 POST JSON
来源：http://nux.zycfv.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hws.daria6918.cn

[R60] 只看 HTTP 状态码
来源：http://unb.birdmap.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mmv.guowangkeji.top

[R61] 磁盘占用
来源：http://ads.fktsv.cn

df -h;  du -sh *
来源：http://hle.yfazqb.com

[R62] 找最占空间的文件
来源：http://djx.zhongyouzk.top

du -ah . | sort -rh | head -10
来源：http://xdq.cashguo.top

[R63] 内存与进程
来源：http://axw.chenzaomai.com

free -h;  ps aux | grep nginx
来源：http://jnj.ehwqpu.com

[R64] 结束进程
来源：http://lsh.uphjek.com

kill -9 $(pgrep -f app.py)
来源：http://bvn.gaohongyu789.top

[R65] 查看端口占用
来源：http://qsb.ywan-chungtsiang.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cex.jianghu66.top

[R66] 定时任务
来源：http://nzy.ivvv.top

crontab -e;  crontab -l
来源：http://cfv.feifeiyinyue.top

[R67] 生成随机十六进制串
来源：http://nve.zhaomingkeji.xyz

openssl rand -hex 16
来源：http://xej.quarkkingdee.top

[R68] 计算文件校验值
来源：http://lkz.feifeiyinyue.top

sha256sum a.txt;  md5sum a.txt
来源：http://dlt.hysaishi.cn

[R69] 生成随机密码
来源：http://zsl.fanxiaobao.xyz

head -c 16 /dev/urandom | base64
来源：http://xxt.havefunace.top

[R70] 时间戳与互转
来源：http://xdr.xingfuxueyuan.xyz

date +%s;  date -d @1700000000
来源：http://egl.ywan-chungtsiang.top

[R71] 日期格式化
来源：http://gzd.zhengqikj.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://agk.yonumen.top

[R72] 等待端口就绪
来源：http://hab.aizwys.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ngo.shzxlz.cn

[R73] 分割大日志
来源：http://hxc.kuanghao11.cn

split -l 1000 big.log part_
来源：http://vnw.vqdsnc.cn

[R74] 批量重命名
来源：http://ztt.hesvh.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yxr.guannengcc.top

[R75] 导出环境变量
来源：http://qim.cucudq.cn

export PATH="$HOME/bin:$PATH"
来源：http://wzk.jinyuanbaomall.cn

[R76] 使用临时文件
来源：http://adt.sxryk.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zrd.cheryme.top

[R77] 读取用户输入
来源：http://lfd.xinyue.icu

read -rp "请输入: " ans
来源：http://adc.hesvh.cn

[R78] 交互式菜单
来源：http://tfz.yuxming.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://vqp.sysykeji.top

[R79] 解析命令行选项
来源：http://lpq.chenlongwang.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ygv.yj202588.top

[R80] 查看脚本执行耗时
来源：http://lah.xylfe.cn

time ./run.sh
来源：http://ztf.tarul.cn

================================================================================
来源：http://ous.sxryk.cn

S. C / C++ 专题
来源：http://jxc.ivvv.top

================================================================================
来源：http://eks.hcnkem.com

[S01] C：Hello World
来源：http://sno.hnqzz.top

#include <stdio.h>
来源：http://lyn.nanxuanxn.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://umy.zhiwuduotai.top

[S02] C：变量与格式化输出
来源：http://tkv.hcnkem.com

int a = 10; printf("%d\n", a);
来源：http://ljo.ydjk.org.cn

[S03] C：读入整数
来源：http://dhm.yueranfly.top

int x; scanf("%d", &x);
来源：http://vzh.chenjidiqi.icu

[S04] C：字符串复制
来源：http://zxg.jiagoushi.top

char dst[32]; strcpy(dst, "hi");
来源：http://xan.gotoacloud.top

[S05] C：字符串长度
来源：http://fwp.hfpthk.cn

strlen(s)
来源：http://arw.quarkkingdee.top

[S06] C：字符串比较
来源：http://ehq.xylfe.cn

strcmp(a, b) == 0
来源：http://nkr.daxiang520.top

[S07] C：数组遍历求和
来源：http://pia.xuetiantiany.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bjp.chenzaomai.com

[S08] C：动态内存分配与释放
来源：http://cjy.chenjidiqi.icu

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fhn.jqgfzy.top

[S09] C：结构体定义与初始化
来源：http://rfx.zdqjudy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://iqf.meibo888.top

[S10] C：指针与解引用
来源：http://nlt.pycfn.com

int *p = &a;  *p = 5;
来源：http://thu.gaohongyu789.top

[S11] C：逐行读文件
来源：http://mop.yj20258.top

FILE *f = fopen("a.txt", "r");
来源：http://ryj.snrcjt.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://dch.zhaomingkeji.xyz

fclose(f);
来源：http://cmf.ctjpmb.com

[S12] C：写文件
来源：http://lkz.ctjpmb.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ygw.vqdsnc.cn

[S13] C：宏定义
来源：http://zvh.hnxiangtu.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wcl.shanyushiyangkeji.top

[S14] C：枚举
来源：http://zlq.gzhubu.top

enum Color { RED, GREEN, BLUE };
来源：http://zax.hammf.cn

[S15] C：类型转换
来源：http://frb.zhijiandao.cn

(double) a / b
来源：http://ygq.hnxiangtu.top

[S16] C：位操作置位
来源：http://tcm.cheryme.top

x |= (1 << 3);
来源：http://vim.hnqzz.top

[S17] C：安全拼接字符串
来源：http://dtp.tian-w.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xxd.zdqjudy.top

[S18] C：命令行参数
来源：http://fie.hnqzz.top

int main(int argc, char **argv)
来源：http://uqa.52xcode.cn

[S19] C：快速排序
来源：http://xjh.zhaomingkeji.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://hju.ppjwa.cn

[S20] C：二分查找
来源：http://kpn.shanyushiyangtech.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zkz.c1oappe.top

[S21] C：字符类别判断
来源：http://ajd.sufxvd.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nrn.316326.xyz

[S22] C：字符串转数字
来源：http://qua.gaohongyu789.top

atoi("42");  strtod("3.14", NULL);
来源：http://fwh.jinyuanbaomall.cn

[S23] C：随机数
来源：http://sfm.nanxinkj.top

srand(time(NULL));  int r = rand() % 100;
来源：http://rgw.0kj1m.cn

[S24] C：获取本地时间
来源：http://ert.svipenyu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://klu.ydzc1.top

[S25] C：内存拷贝
来源：http://gok.snrcjt.cn

memcpy(dst, src, n);
来源：http://ded.feifeiyinyue.top

[S26] C：内存清零
来源：http://hcd.vqdsnc.cn

memset(a, 0, sizeof a);
来源：http://vyu.birdmap.top

[S27] C：定义常量
来源：http://orc.haohaochexian.top

const double PI = 3.14159;
来源：http://rho.pengpengdd.cyou

[S28] C：静态变量
来源：http://yna.chenjidiqi.icu

static int counter = 0;
来源：http://oze.xylfe.cn

[S29] C：变参函数
来源：http://tqk.yueranfly.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yea.chenzaomai.com

[S30] C：头文件保护
来源：http://pqo.jiagoushi.top

#ifndef X_H
来源：http://vfi.andypj.xyz

#define X_H
来源：http://kvw.mhx1999.top

#endif
来源：http://jrh.chenlongwang.top

[S31] C++：Hello World
来源：http://sar.yanxiufei.cn

#include <iostream>
来源：http://pdi.jinghuilouyu.cn

int main() { std::cout << "Hello\n"; }
来源：http://ivu.zdbjq.cn

[S32] C++：字符串
来源：http://ghm.cqqwz.cn

std::string s = "hi";  s += "!";
来源：http://xxh.nwbrower.top

[S33] C++：vector 增删
来源：http://dxi.pengpengdd.cyou

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ppc.hywenlv.cn

[S34] C++：遍历 vector
来源：http://sdw.jiagoushi.top

for (auto &x : v) { std::cout << x; }
来源：http://fva.yuxming.cn

[S35] C++：map
来源：http://bln.pengpengdd.cyou

std::map<std::string, int> m;  m["a"] = 1;
来源：http://eus.shanyushiyangtech.top

[S36] C++：unordered_map
来源：http://ylt.fzhhl.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nct.cdnleiting.top

[S37] C++：set
来源：http://xfb.jlsjyb.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qny.xingfuxueyuan.xyz

[S38] C++：排序
来源：http://qra.c1oappe.top

std::sort(v.begin(), v.end());
来源：http://ype.hongshengwenyu.top

[S39] C++：自定义比较器排序
来源：http://opa.wangshuangyany.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qvh.mhx1999.top

[S40] C++：查找元素
来源：http://mvl.quarkkingdee.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xmb.52xcode.cn

[S41] C++：类与构造函数
来源：http://fol.pycfn.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cut.zhijiandao.cn

[S42] C++：继承与虚函数
来源：http://svl.zhiwuduotai.top

class B : public Base { public: void f() override {} };
来源：http://trc.yfazqb.com

[S43] C++：智能指针
来源：http://tgy.andypj.xyz

auto p = std::make_unique<int>(5);
来源：http://jqz.meibo888.top

[S44] C++：引用传参
来源：http://zsd.smart0.xyz

void inc(int &x) { ++x; }
来源：http://vkm.feifeiyinyue.top

[S45] C++：lambda
来源：http://ryw.hywenlv.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fwr.sysykeji.top

[S46] C++：函数模板
来源：http://jhr.jiagoushi.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cwt.redwolf501.top


<!-- 参考信息 -->
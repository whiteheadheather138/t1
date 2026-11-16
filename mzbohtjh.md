代发 wailian999

[Q63] 开启事务
来源：http://vvm.jinghuilouyu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://hpj.ybcxt.top

[Q64] 提交事务
来源：http://cch.aibaodan.cn

COMMIT;
来源：http://vya.ehwqpu.com

[Q65] 回滚事务
来源：http://cjh.xinyue.icu

ROLLBACK;
来源：http://xfg.ehwqpu.com

[Q66] 行锁查询
来源：http://ugh.jqgfzy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://stz.hywenlv.cn

[Q67] 设置隔离级别
来源：http://ndt.aibaodan.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xqr.xuetiantiany.cn

[Q68] 保存点
来源：http://enw.fanxiaobao.xyz

SAVEPOINT sp1;
来源：http://akv.wangshuangyany.cn

ROLLBACK TO sp1;
来源：http://gkv.kuanghao11.cn

[Q69] 查看执行计划
来源：http://mar.sweek.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ney.xuanzx.com

[Q70] 更新统计信息
来源：http://pxy.zhongyouzk.top

ANALYZE TABLE users;
来源：http://ytg.haohaochexian.top

[Q71] 查看建表语句
来源：http://mcs.hongshengwenyu.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xam.yuanzhike.top

[Q72] 查看索引
来源：http://uxd.hnxiangtu.top

SHOW INDEX FROM users;
来源：http://cyt.quarkkingdee.top

[Q73] 查看表状态
来源：http://smf.0kj1m.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://zbu.yanxiufei.cn

[Q74] 强制使用索引
来源：http://uqk.sjlbkw.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fli.daxiang520.top

[Q75] 日期格式化
来源：http://sxf.gotoacloud.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rap.hnxiangtu.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://uez.sweek.top

[Q76] 按天统计
来源：http://gqs.quarkkingdee.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ibs.pengpengdd.cyou

[Q77] 时间加减
来源：http://fys.jlsjyb.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gxr.jinqigfzy.top

[Q78] 当前时间
来源：http://epr.aizwys.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xbx.ppjwa.cn

[Q79] 字符串拼接
来源：http://cqa.aizwys.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qyl.gzhubu.top

[Q80] 字符串截取
来源：http://vyy.xuanzx.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zdg.316326.xyz

[Q81] 字符串替换
来源：http://pjj.vehdjk.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ded.gotoacloud.top

[Q82] 字符长度与字节长度
来源：http://ohr.sysykeji.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jiz.52xcode.cn

[Q83] 大小写转换
来源：http://lwj.chenjidiqi.icu

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cpk.jlsjyb.cn

[Q84] 去除首尾空格
来源：http://zek.shuidangran.top

SELECT TRIM(name) FROM users;
来源：http://dgy.quarkkingdee.top

[Q85] 数值取整
来源：http://eqh.yongpay.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zzh.mhx1999.top

[Q86] 读取 JSON 字段
来源：http://bck.hnqzz.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xuq.yuanzhike.top

[Q87] JSON 字段做条件
来源：http://kyp.cqqwz.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tec.xziqi.cn

[Q88] 行转列（条件聚合）
来源：http://yto.pycfn.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mvr.ivvv.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bch.haohaochexian.top

[Q89] 判断表是否存在
来源：http://tmv.svipenyu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xgi.hammf.cn

[Q90] 生成序号列
来源：http://ojg.gaohongyu789.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://isc.hnxiangtu.top

================================================================================
来源：http://tzx.hammf.cn

R. Bash 专题
来源：http://irp.hywenlv.cn

================================================================================
来源：http://vbv.cucudq.cn

[R01] shebang 与严格模式
来源：http://dtd.hcnkem.com

#!/usr/bin/env bash
来源：http://tak.tanke756.top

set -euo pipefail
来源：http://itf.andypj.xyz

[R02] 变量赋值与使用
来源：http://pjc.fengsongda.top

name="Tom"; echo "$name"
来源：http://hwv.wangshuangyany.cn

[R03] 只读变量
来源：http://auh.ctjpmb.com

readonly PI=3.14
来源：http://icq.zhiwuduotai.top

[R04] 位置参数
来源：http://uuk.redwolf501.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zcp.sjlbkw.cn

[R05] 参数默认值
来源：http://nrj.hnxiangtu.top

name="${1:-default}"
来源：http://gua.cucudq.cn

[R06] 判断命令是否存在
来源：http://ifh.tianlin.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cjx.nanxuanxn.top

[R07] if 判断文件
来源：http://hyk.hammf.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://owl.uphjek.com

[R08] 数值比较
来源：http://lts.pycfn.com

if (( a > b )); then echo "a 更大"; fi
来源：http://ytn.fzhhl.top

[R09] 字符串比较
来源：http://drg.zhengqikj.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tjk.xingfuxueyuan.xyz

[R10] 正则匹配
来源：http://yhc.jinqigufen.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://olw.iojbl.cn

[R11] case 多分支
来源：http://ekh.tanke756.top

case "$1" in
来源：http://bqq.hnqzz.top

start) echo "启动" ;;
来源：http://qzy.yj20258.top

stop)  echo "停止" ;;
来源：http://jwz.cashguo.top

*)     echo "未知命令" ;;
来源：http://lyh.yj20258888.top

esac
来源：http://izc.gzhubu.top

[R12] for 遍历文件
来源：http://bek.xuanzx.com

for f in *.txt; do echo "$f"; done
来源：http://nlk.cheryme.top

[R13] for 计数循环
来源：http://iuk.hfpthk.cn

for i in {1..10}; do echo "$i"; done
来源：http://gfk.jqgfzy.top

[R14] C 风格 for
来源：http://mnt.svipenyu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fhh.jqgufenzy.top

[R15] while 逐行读文件
来源：http://cns.yfazqb.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zja.fzhhl.top

[R16] until 等待条件
来源：http://vfo.yuanzhike.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://snq.zhoulong.xyz

[R17] 数组定义与取值
来源：http://tta.c1oappe.top

arr=(a b c); echo "${arr[0]}"
来源：http://lgv.zhengqikj.top

[R18] 遍历数组
来源：http://psh.zhijiandao.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bbg.fzhhl.top

[R19] 数组长度
来源：http://zzx.wangdashe.top

echo "${#arr[@]}"
来源：http://bgm.yj20258888.top

[R20] 关联数组（字典）
来源：http://xsw.nanxinkj.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://boy.hnxiangtu.top

[R21] 字符串长度
来源：http://fxa.ppjwa.cn

echo "${#s}"
来源：http://mzi.gotoacloud.top

[R22] 截取子串
来源：http://rjm.zhiwuduotai.top

echo "${s:0:5}"
来源：http://zgy.smart0.xyz

[R23] 字符串替换
来源：http://sxb.316326.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fys.xinyue.icu

[R24] 大小写转换
来源：http://zcw.yuanzhike.top

echo "${s^^}"; echo "${s,,}"
来源：http://fwz.yuxming.cn

[R25] 去后缀 / 去前缀
来源：http://qrq.yfazqb.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://ewh.ctjpmb.com

[R26] 命令替换
来源：http://yxw.smart0.xyz

now=$(date +%F); echo "$now"
来源：http://eco.hesvh.cn

[R27] 算术展开
来源：http://djn.hesvh.cn

echo $((1 + 2 * 3))
来源：http://ibx.chenjidiqi.icu

[R28] 浮点运算
来源：http://vim.shanyushiyangkeji.top

echo "scale=2; 10/3" | bc
来源：http://nyq.guannengcc.top

[R29] 定义函数
来源：http://ycp.mhx1999.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://euf.gogol.net.cn

[R30] 函数返回状态码
来源：http://fym.epnwcf.com

f() { return 0; }; f || echo "失败了"
来源：http://kvz.9152youxi.cn

[R31] 局部变量
来源：http://xfu.pycfn.com

f() { local x=1; echo "$x"; }
来源：http://xec.hysaishi.cn

[R32] 参数个数校验
来源：http://mac.hesvh.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mai.zycfv.cn

[R33] 捕获错误并提示行号
来源：http://mxy.yangfankeji.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ile.sjlbkw.cn

[R34] 退出时清理
来源：http://bxm.andypj.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://jid.yj202588.top

[R35] 后台执行并等待
来源：http://mzd.tianlin.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://usu.hywenlv.cn

[R36] 并发执行多个任务
来源：http://pvc.nwbrower.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://diy.aibaodan.cn

[R37] 把输出赋给变量
来源：http://olq.bjfxy.top

files=$(ls -1)
来源：http://wkm.iojbl.cn

[R38] 管道串联
来源：http://oav.haohaochexian.top

cat a.txt | grep -i error | wc -l
来源：http://ltj.wangdashe.top

[R39] 重定向标准输出与错误
来源：http://csn.xziqi.cn

cmd > out.log 2>&1
来源：http://eij.ydjk.org.cn

[R40] 追加写日志
来源：http://tnt.ydzc1.top

echo "log" >> out.log
来源：http://ius.gogol.net.cn

[R41] 丢弃输出
来源：http://ssu.hcnkem.com

cmd >/dev/null 2>&1
来源：http://agl.fanxiaobao.xyz

[R42] 输入重定向
来源：http://ype.dashuyun.cn

wc -l < a.txt
来源：http://roy.jinqigufen.top

[R43] 按名字查找文件
来源：http://rdj.52xcode.cn

find . -name "*.log" -type f
来源：http://esn.bbcook.cn

[R44] 按修改时间查找
来源：http://vie.tian-w.cn

find . -mtime -7 -type f
来源：http://lss.guowangkeji.top

[R45] 批量删除
来源：http://ayi.yvedp.cn

find . -name "*.tmp" -delete
来源：http://gcj.sysykeji.top

[R46] 递归替换文件内容
来源：http://zov.yuanzhike.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pgg.ctjpmb.com

[R47] sed 单行替换
来源：http://szy.ydjk.org.cn

sed -i 's/foo/bar/g' a.txt
来源：http://zpe.wangdashe.top

[R48] awk 取指定列
来源：http://ebx.hywenlv.cn

awk '{print $1, $3}' a.txt
来源：http://lyf.hysaishi.cn

[R49] awk 带条件
来源：http://lfr.zycfv.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://aje.xziqi.cn

[R50] awk 求和
来源：http://kgu.ehwqpu.com

awk '{s += $2} END {print s}' a.txt
来源：http://tam.xinyue.icu

[R51] 排序去重取前几
来源：http://uel.pycfn.com

sort a.txt | uniq -c | sort -rn | head
来源：http://wbx.hcnkem.com

[R52] 统计行数
来源：http://ret.xylfe.cn

wc -l a.txt
来源：http://kdp.snrcjt.cn

[R53] 查看文件头与实时尾
来源：http://nrs.0kj1m.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nwr.redwolf501.top

[R54] 比较两个文件
来源：http://inc.ehwqpu.com

diff a.txt b.txt
来源：http://fhr.shzxlz.cn

[R55] 压缩与解压
来源：http://wya.yangfankeji.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://faq.iojbl.cn

[R56] 远程拷贝
来源：http://kpi.xylfe.cn

scp file user@host:/path/
来源：http://bub.zdbjq.cn

[R57] 远程执行命令
来源：http://ckt.cqqwz.cn

ssh user@host 'uptime'
来源：http://qxw.yangfankeji.com

[R58] 下载文件
来源：http://fdm.gotoacloud.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rdx.zhixingplan.top

[R59] 发 POST JSON
来源：http://ynf.fehbvm.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ono.jinqigufen.top

[R60] 只看 HTTP 状态码
来源：http://ick.mhx1999.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pzp.hongshengwenyu.top

[R61] 磁盘占用
来源：http://las.chenjidiqi.icu

df -h;  du -sh *
来源：http://uxt.hongshengwenyu.top

[R62] 找最占空间的文件
来源：http://bok.dashuyun.cn

du -ah . | sort -rh | head -10
来源：http://mda.yvedp.cn

[R63] 内存与进程
来源：http://xlg.fanxiaobao.xyz

free -h;  ps aux | grep nginx
来源：http://jkc.xuanzx.com

[R64] 结束进程
来源：http://rtm.aibaodan.cn

kill -9 $(pgrep -f app.py)
来源：http://zdm.zhongyouzk.top

[R65] 查看端口占用
来源：http://afp.dianchejie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wiy.jianghu66.top

[R66] 定时任务
来源：http://jue.zhijiandao.cn

crontab -e;  crontab -l
来源：http://odn.yj20258888.top

[R67] 生成随机十六进制串
来源：http://pjq.sweek.top

openssl rand -hex 16
来源：http://poe.zdbjq.cn

[R68] 计算文件校验值
来源：http://xfs.hammf.cn

sha256sum a.txt;  md5sum a.txt
来源：http://nwb.chenlongwang.top

[R69] 生成随机密码
来源：http://twa.xziqi.cn

head -c 16 /dev/urandom | base64
来源：http://eil.zhaomingkeji.xyz

[R70] 时间戳与互转
来源：http://vgs.jinghuilouyu.cn

date +%s;  date -d @1700000000
来源：http://lkx.jinyuanbaomall.cn

[R71] 日期格式化
来源：http://geo.tianlin.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://bsv.zhengqikj.top

[R72] 等待端口就绪
来源：http://yad.guannengcc.top

until nc -z localhost 3306; do sleep 1; done
来源：http://fzl.hfpthk.cn

[R73] 分割大日志
来源：http://req.yfazqb.com

split -l 1000 big.log part_
来源：http://zyt.cqqwz.cn

[R74] 批量重命名
来源：http://rif.tian-w.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lzq.dianchejie.cn

[R75] 导出环境变量
来源：http://slc.ywan-chungtsiang.top

export PATH="$HOME/bin:$PATH"
来源：http://khm.mhx1999.top

[R76] 使用临时文件
来源：http://pmo.ppjwa.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://smo.meibo888.top

[R77] 读取用户输入
来源：http://ugc.cheryme.top

read -rp "请输入: " ans
来源：http://xlc.fengsongda.top

[R78] 交互式菜单
来源：http://yil.guannengcc.top

select opt in a b c; do echo "$opt"; break; done
来源：http://biv.ivvv.top

[R79] 解析命令行选项
来源：http://bfz.zhijiandao.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lub.ppjwa.cn

[R80] 查看脚本执行耗时
来源：http://mgl.uphjek.com

time ./run.sh
来源：http://ztc.sysykeji.top

================================================================================
来源：http://thb.ywan-chungtsiang.top

S. C / C++ 专题
来源：http://jqj.shangyingyoupin.top

================================================================================
来源：http://lfm.ydzc1.top

[S01] C：Hello World
来源：http://mti.ehwqpu.com

#include <stdio.h>
来源：http://oal.cqqwz.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xce.yongpay.top

[S02] C：变量与格式化输出
来源：http://mrd.xinyue.icu

int a = 10; printf("%d\n", a);
来源：http://gcw.cucudq.cn

[S03] C：读入整数
来源：http://ovb.tanke756.top

int x; scanf("%d", &x);
来源：http://ktz.c1oappe.top

[S04] C：字符串复制
来源：http://cts.jlsjyb.cn

char dst[32]; strcpy(dst, "hi");
来源：http://sam.yuanzhike.top

[S05] C：字符串长度
来源：http://kfx.daria6918.cn

strlen(s)
来源：http://sgp.ydjk.org.cn

[S06] C：字符串比较
来源：http://fhx.tarul.cn

strcmp(a, b) == 0
来源：http://jte.daria6918.cn

[S07] C：数组遍历求和
来源：http://gjm.zhongyouzk.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kyy.yj20258.top

[S08] C：动态内存分配与释放
来源：http://opu.jqgufenzy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://sms.hesvh.cn

[S09] C：结构体定义与初始化
来源：http://hcu.sxryk.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rzl.fzhhl.top

[S10] C：指针与解引用
来源：http://bmc.xylfe.cn

int *p = &a;  *p = 5;
来源：http://qyx.wangshuangyany.cn

[S11] C：逐行读文件
来源：http://ttz.zhengqikj.top

FILE *f = fopen("a.txt", "r");
来源：http://mdx.9152youxi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://evy.feifeiyinyue.top

fclose(f);
来源：http://kxk.yongpay.top

[S12] C：写文件
来源：http://gfc.yangfankeji.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wts.0kj1m.cn

[S13] C：宏定义
来源：http://tcl.jyoumei.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sbu.yuanzhike.top

[S14] C：枚举
来源：http://rml.ivvv.top

enum Color { RED, GREEN, BLUE };
来源：http://oqr.epnwcf.com

[S15] C：类型转换
来源：http://oum.ybcxt.top

(double) a / b
来源：http://ihr.gotoacloud.top

[S16] C：位操作置位
来源：http://ivz.yuanzhike.top

x |= (1 << 3);
来源：http://hmk.nanxinkj.top

[S17] C：安全拼接字符串
来源：http://bdz.jlsjyb.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kdw.ybcxt.top

[S18] C：命令行参数
来源：http://ahk.iojbl.cn

int main(int argc, char **argv)
来源：http://ksf.daxiang520.top

[S19] C：快速排序
来源：http://ojc.xingfuxueyuan.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://mpm.shanyushiyangtech.top

[S20] C：二分查找
来源：http://znd.wangshuangyany.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://oun.yj20258888.top

[S21] C：字符类别判断
来源：http://uhx.9152youxi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fka.zdqjudy.top

[S22] C：字符串转数字
来源：http://sgo.52xcode.cn

atoi("42");  strtod("3.14", NULL);
来源：http://akf.hcnkem.com

[S23] C：随机数
来源：http://kwb.xylfe.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zhy.hesvh.cn

[S24] C：获取本地时间
来源：http://pxn.sysykeji.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rrq.smart0.xyz

[S25] C：内存拷贝
来源：http://noi.birdmap.top

memcpy(dst, src, n);
来源：http://lwi.wangshuangyany.cn

[S26] C：内存清零
来源：http://ivx.ivvv.top

memset(a, 0, sizeof a);
来源：http://tjv.tian-w.cn

[S27] C：定义常量
来源：http://ppc.ehwqpu.com

const double PI = 3.14159;
来源：http://zfc.ydjk.org.cn

[S28] C：静态变量
来源：http://fau.fzhhl.top

static int counter = 0;
来源：http://luw.andypj.xyz

[S29] C：变参函数
来源：http://tug.sweek.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xfz.pengpengdd.cyou

[S30] C：头文件保护
来源：http://tuc.ydzc1.top

#ifndef X_H
来源：http://usz.jianghu66.top

#define X_H
来源：http://dzq.shanyushiyangkeji.top

#endif
来源：http://tgi.gaohongyu789.top

[S31] C++：Hello World
来源：http://dlk.bjfxy.top

#include <iostream>
来源：http://krm.zhijiandao.cn

int main() { std::cout << "Hello\n"; }
来源：http://lcs.jinghuilouyu.cn

[S32] C++：字符串
来源：http://lgo.yj20258.top

std::string s = "hi";  s += "!";
来源：http://tbk.nanxinkj.top


<!-- 参考信息 -->
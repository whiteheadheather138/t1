代发 wailian999

[Q61] 移动平均
来源：http://tdk.yongpay.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jsw.tian-w.cn

[Q62] 分组占比
来源：http://xdp.fanxiaobao.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wtx.yonumen.top

[Q63] 开启事务
来源：http://gpq.52xcode.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ins.yuxming.cn

[Q64] 提交事务
来源：http://yjt.0kj1m.cn

COMMIT;
来源：http://acp.zhengqikj.top

[Q65] 回滚事务
来源：http://ilr.9152youxi.cn

ROLLBACK;
来源：http://tjj.hnqzz.top

[Q66] 行锁查询
来源：http://bsp.fktsv.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bgr.bjfxy.top

[Q67] 设置隔离级别
来源：http://vwc.zhiwuduotai.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://iod.pengpengdd.cyou

[Q68] 保存点
来源：http://mnv.nanxinkj.top

SAVEPOINT sp1;
来源：http://ldp.feifeiyinyue.top

ROLLBACK TO sp1;
来源：http://foe.yfazqb.com

[Q69] 查看执行计划
来源：http://teb.fengsongda.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fxk.sjlbkw.cn

[Q70] 更新统计信息
来源：http://mcn.fehbvm.com

ANALYZE TABLE users;
来源：http://bud.hnqzz.top

[Q71] 查看建表语句
来源：http://dat.jlsjyb.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mjg.havefunace.top

[Q72] 查看索引
来源：http://myo.yangfankeji.com

SHOW INDEX FROM users;
来源：http://asw.hywenlv.cn

[Q73] 查看表状态
来源：http://hwf.hysaishi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://grm.wangdashe.top

[Q74] 强制使用索引
来源：http://csx.shzxlz.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gbb.fehbvm.com

[Q75] 日期格式化
来源：http://jal.hysaishi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dbz.9152youxi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fbo.0kj1m.cn

[Q76] 按天统计
来源：http://acz.sxryk.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://itu.yongpay.top

[Q77] 时间加减
来源：http://giq.feifeiyinyue.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://don.vqdsnc.cn

[Q78] 当前时间
来源：http://jjl.zhixingplan.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://alu.dashuyun.cn

[Q79] 字符串拼接
来源：http://xxy.ywan-chungtsiang.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hny.zdbjq.cn

[Q80] 字符串截取
来源：http://nqr.vqdsnc.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nut.gzhubu.top

[Q81] 字符串替换
来源：http://fug.gogol.net.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wys.52xcode.cn

[Q82] 字符长度与字节长度
来源：http://rmi.gogol.net.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://irl.shzxlz.cn

[Q83] 大小写转换
来源：http://csf.zhongyouzk.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bah.dianchejie.cn

[Q84] 去除首尾空格
来源：http://lnr.cashguo.top

SELECT TRIM(name) FROM users;
来源：http://awy.nanxuanxn.top

[Q85] 数值取整
来源：http://pop.vehdjk.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://joi.zdbjq.cn

[Q86] 读取 JSON 字段
来源：http://zzm.shangyingyoupin.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gmn.kuanghao11.cn

[Q87] JSON 字段做条件
来源：http://ruk.xinyue.icu

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://sgt.gotoacloud.top

[Q88] 行转列（条件聚合）
来源：http://mlp.cucudq.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vxw.ppjwa.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://oeq.zdbjq.cn

[Q89] 判断表是否存在
来源：http://tju.tianlin.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mvd.xuanzx.com

[Q90] 生成序号列
来源：http://gua.zhaomingkeji.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qsb.meibo888.top

================================================================================
来源：http://szt.yuanzhike.top

R. Bash 专题
来源：http://rqz.jinqigfzy.top

================================================================================
来源：http://akh.ydjk.org.cn

[R01] shebang 与严格模式
来源：http://aqv.xingfuxueyuan.xyz

#!/usr/bin/env bash
来源：http://xem.jqgufenzy.top

set -euo pipefail
来源：http://lxf.sweek.top

[R02] 变量赋值与使用
来源：http://fnx.ppjwa.cn

name="Tom"; echo "$name"
来源：http://oal.shanyushiyangtech.top

[R03] 只读变量
来源：http://jta.quarkkingdee.top

readonly PI=3.14
来源：http://esw.hnqzz.top

[R04] 位置参数
来源：http://muf.tian-w.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://uda.iojbl.cn

[R05] 参数默认值
来源：http://jcq.vqdsnc.cn

name="${1:-default}"
来源：http://xre.ydzc1.top

[R06] 判断命令是否存在
来源：http://nvn.nanxuanxn.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uzg.yj202588.top

[R07] if 判断文件
来源：http://fco.aibaodan.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kxy.gzhubu.top

[R08] 数值比较
来源：http://gsm.jinqigufen.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ozp.ybcxt.top

[R09] 字符串比较
来源：http://bjy.ybcxt.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zeq.hesvh.cn

[R10] 正则匹配
来源：http://nqs.jianghu66.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xxu.c1oappe.top

[R11] case 多分支
来源：http://lth.sweek.top

case "$1" in
来源：http://djh.zhiwuduotai.top

start) echo "启动" ;;
来源：http://xco.9152youxi.cn

stop)  echo "停止" ;;
来源：http://fjz.aizwys.cn

*)     echo "未知命令" ;;
来源：http://igm.iojbl.cn

esac
来源：http://ddn.jqgufenzy.top

[R12] for 遍历文件
来源：http://tgi.52xcode.cn

for f in *.txt; do echo "$f"; done
来源：http://csw.aizwys.cn

[R13] for 计数循环
来源：http://kzd.jyoumei.cn

for i in {1..10}; do echo "$i"; done
来源：http://mmr.sjlbkw.cn

[R14] C 风格 for
来源：http://pcg.hnqzz.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sgs.316326.xyz

[R15] while 逐行读文件
来源：http://whj.jqgfzy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cfb.snrcjt.cn

[R16] until 等待条件
来源：http://fxo.epnwcf.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qky.shanyushiyangkeji.top

[R17] 数组定义与取值
来源：http://fnn.xuetiantiany.cn

arr=(a b c); echo "${arr[0]}"
来源：http://cnw.yj20258.top

[R18] 遍历数组
来源：http://mbv.52xcode.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sjr.cheryme.top

[R19] 数组长度
来源：http://mfa.iojbl.cn

echo "${#arr[@]}"
来源：http://cui.yj202588.top

[R20] 关联数组（字典）
来源：http://xlw.pengpengdd.cyou

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wkh.xuanzx.com

[R21] 字符串长度
来源：http://mzz.yfazqb.com

echo "${#s}"
来源：http://jqf.aibaodan.cn

[R22] 截取子串
来源：http://mnz.cucudq.cn

echo "${s:0:5}"
来源：http://ryw.hammf.cn

[R23] 字符串替换
来源：http://zdb.sysykeji.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nsi.quarkkingdee.top

[R24] 大小写转换
来源：http://kxs.jianghu66.top

echo "${s^^}"; echo "${s,,}"
来源：http://ikh.yj202588.top

[R25] 去后缀 / 去前缀
来源：http://lgr.316326.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://phz.haohaochexian.top

[R26] 命令替换
来源：http://itq.vqdsnc.cn

now=$(date +%F); echo "$now"
来源：http://vgr.tarul.cn

[R27] 算术展开
来源：http://ikv.zhiwuduotai.top

echo $((1 + 2 * 3))
来源：http://cli.tianlin.xyz

[R28] 浮点运算
来源：http://ukz.daria6918.cn

echo "scale=2; 10/3" | bc
来源：http://wrt.zhaomingkeji.xyz

[R29] 定义函数
来源：http://pfg.xuetiantiany.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fjj.tarul.cn

[R30] 函数返回状态码
来源：http://xvp.zhongyouzk.top

f() { return 0; }; f || echo "失败了"
来源：http://kaa.daxiang520.top

[R31] 局部变量
来源：http://aep.birdmap.top

f() { local x=1; echo "$x"; }
来源：http://jcf.dashuyun.cn

[R32] 参数个数校验
来源：http://les.fehbvm.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bnk.sufxvd.cn

[R33] 捕获错误并提示行号
来源：http://rdt.guannengcc.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vsg.guowangkeji.top

[R34] 退出时清理
来源：http://bvy.zhongyouzk.top

trap 'rm -f "$tmp"' EXIT
来源：http://bcv.wangdashe.top

[R35] 后台执行并等待
来源：http://mcm.c1oappe.top

sleep 5 & pid=$!; wait "$pid"
来源：http://kwk.c1oappe.top

[R36] 并发执行多个任务
来源：http://cqj.vehdjk.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zjd.uphjek.com

[R37] 把输出赋给变量
来源：http://yxu.hesvh.cn

files=$(ls -1)
来源：http://hfh.ywan-chungtsiang.top

[R38] 管道串联
来源：http://eez.hfpthk.cn

cat a.txt | grep -i error | wc -l
来源：http://xfq.pengpengdd.cyou

[R39] 重定向标准输出与错误
来源：http://fwy.pycfn.com

cmd > out.log 2>&1
来源：http://zck.ywan-chungtsiang.top

[R40] 追加写日志
来源：http://gwt.yangfankeji.com

echo "log" >> out.log
来源：http://tiq.zhijiandao.cn

[R41] 丢弃输出
来源：http://bym.kuanghao11.cn

cmd >/dev/null 2>&1
来源：http://hbp.andypj.xyz

[R42] 输入重定向
来源：http://tfg.9152youxi.cn

wc -l < a.txt
来源：http://jmm.ywan-chungtsiang.top

[R43] 按名字查找文件
来源：http://qea.quarkkingdee.top

find . -name "*.log" -type f
来源：http://fbk.gogol.net.cn

[R44] 按修改时间查找
来源：http://lnu.sysykeji.top

find . -mtime -7 -type f
来源：http://zkh.yanxiufei.cn

[R45] 批量删除
来源：http://cft.xylfe.cn

find . -name "*.tmp" -delete
来源：http://cpr.ybcxt.top

[R46] 递归替换文件内容
来源：http://enz.xziqi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cqi.yj20258.top

[R47] sed 单行替换
来源：http://kfw.tarul.cn

sed -i 's/foo/bar/g' a.txt
来源：http://grb.zhaomingkeji.xyz

[R48] awk 取指定列
来源：http://vzl.epnwcf.com

awk '{print $1, $3}' a.txt
来源：http://uzi.yj202588.top

[R49] awk 带条件
来源：http://jnh.daxiang520.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vqy.zhixingplan.top

[R50] awk 求和
来源：http://ozm.sjlbkw.cn

awk '{s += $2} END {print s}' a.txt
来源：http://yyn.52xcode.cn

[R51] 排序去重取前几
来源：http://xfj.hesvh.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://yrs.jianghu66.top

[R52] 统计行数
来源：http://phg.tarul.cn

wc -l a.txt
来源：http://lvp.gaohongyu789.top

[R53] 查看文件头与实时尾
来源：http://tyo.yuxming.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://few.vqdsnc.cn

[R54] 比较两个文件
来源：http://eqk.52xcode.cn

diff a.txt b.txt
来源：http://hom.yueranfly.top

[R55] 压缩与解压
来源：http://enq.fktsv.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://emh.shuidangran.top

[R56] 远程拷贝
来源：http://qtb.tarul.cn

scp file user@host:/path/
来源：http://sxg.hcnkem.com

[R57] 远程执行命令
来源：http://npq.feifeiyinyue.top

ssh user@host 'uptime'
来源：http://kun.havefunace.top

[R58] 下载文件
来源：http://api.cucudq.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cgu.gaohongyu789.top

[R59] 发 POST JSON
来源：http://dii.sweek.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://udn.gotoacloud.top

[R60] 只看 HTTP 状态码
来源：http://rgb.yongpay.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qga.yuanzhike.top

[R61] 磁盘占用
来源：http://pnr.jinyuanbaomall.cn

df -h;  du -sh *
来源：http://dxf.shzxlz.cn

[R62] 找最占空间的文件
来源：http://inr.xingfuxueyuan.xyz

du -ah . | sort -rh | head -10
来源：http://ydw.ydzc1.top

[R63] 内存与进程
来源：http://lbu.c1oappe.top

free -h;  ps aux | grep nginx
来源：http://isj.pycfn.com

[R64] 结束进程
来源：http://ojy.guannengcc.top

kill -9 $(pgrep -f app.py)
来源：http://gpp.ctjpmb.com

[R65] 查看端口占用
来源：http://hor.tianlin.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://uws.zhixingplan.top

[R66] 定时任务
来源：http://lma.xylfe.cn

crontab -e;  crontab -l
来源：http://osa.ppjwa.cn

[R67] 生成随机十六进制串
来源：http://gwt.epnwcf.com

openssl rand -hex 16
来源：http://sbu.fengsongda.top

[R68] 计算文件校验值
来源：http://xxv.xziqi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://rot.fzhhl.top

[R69] 生成随机密码
来源：http://gfq.sufxvd.cn

head -c 16 /dev/urandom | base64
来源：http://tus.wangdashe.top

[R70] 时间戳与互转
来源：http://gil.chenjidiqi.icu

date +%s;  date -d @1700000000
来源：http://fzm.zhaomingkeji.xyz

[R71] 日期格式化
来源：http://zgz.jianghu66.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://sye.dianchejie.cn

[R72] 等待端口就绪
来源：http://oqu.vehdjk.com

until nc -z localhost 3306; do sleep 1; done
来源：http://myq.smart0.xyz

[R73] 分割大日志
来源：http://wfr.cdnleiting.top

split -l 1000 big.log part_
来源：http://hpt.chenzaomai.com

[R74] 批量重命名
来源：http://wsf.vqdsnc.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fgv.redwolf501.top

[R75] 导出环境变量
来源：http://itu.ybcxt.top

export PATH="$HOME/bin:$PATH"
来源：http://wis.fktsv.cn

[R76] 使用临时文件
来源：http://nzt.jqgufenzy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://van.yj20258.top

[R77] 读取用户输入
来源：http://bni.cashguo.top

read -rp "请输入: " ans
来源：http://jld.yvedp.cn

[R78] 交互式菜单
来源：http://eov.chenlongwang.top

select opt in a b c; do echo "$opt"; break; done
来源：http://tfm.zhaomingkeji.xyz

[R79] 解析命令行选项
来源：http://yda.yonumen.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://iiw.nwbrower.top

[R80] 查看脚本执行耗时
来源：http://luu.ywan-chungtsiang.top

time ./run.sh
来源：http://hyu.ehwqpu.com

================================================================================
来源：http://tme.dianchejie.cn

S. C / C++ 专题
来源：http://cug.hywenlv.cn

================================================================================
来源：http://vzr.andypj.xyz

[S01] C：Hello World
来源：http://exs.chenzaomai.com

#include <stdio.h>
来源：http://lin.uphjek.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://dth.jiagoushi.top

[S02] C：变量与格式化输出
来源：http://ohp.ywan-chungtsiang.top

int a = 10; printf("%d\n", a);
来源：http://ajc.ydjk.org.cn

[S03] C：读入整数
来源：http://xzd.vqdsnc.cn

int x; scanf("%d", &x);
来源：http://vxd.daxiang520.top

[S04] C：字符串复制
来源：http://euy.vqdsnc.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xxc.gogol.net.cn

[S05] C：字符串长度
来源：http://jma.haohaochexian.top

strlen(s)
来源：http://oqq.yangfankeji.com

[S06] C：字符串比较
来源：http://qis.sufxvd.cn

strcmp(a, b) == 0
来源：http://rho.chenjidiqi.icu

[S07] C：数组遍历求和
来源：http://fkk.9152youxi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ejo.316326.xyz

[S08] C：动态内存分配与释放
来源：http://bdt.yangfankeji.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://csr.redwolf501.top

[S09] C：结构体定义与初始化
来源：http://gpx.wangdashe.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vgk.ybcxt.top

[S10] C：指针与解引用
来源：http://hdn.gzhubu.top

int *p = &a;  *p = 5;
来源：http://grn.aibaodan.cn

[S11] C：逐行读文件
来源：http://yhf.tianlin.xyz

FILE *f = fopen("a.txt", "r");
来源：http://dry.pycfn.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://ikk.vqdsnc.cn

fclose(f);
来源：http://bhv.jiagoushi.top

[S12] C：写文件
来源：http://pbs.ctjpmb.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://txy.smart0.xyz

[S13] C：宏定义
来源：http://zre.zhijiandao.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vdp.jianghu66.top

[S14] C：枚举
来源：http://dni.daxiang520.top

enum Color { RED, GREEN, BLUE };
来源：http://wdj.haohaochexian.top

[S15] C：类型转换
来源：http://chj.zhaomingkeji.xyz

(double) a / b
来源：http://vwo.kuanghao11.cn

[S16] C：位操作置位
来源：http://mwq.sjlbkw.cn

x |= (1 << 3);
来源：http://lzg.yongpay.top

[S17] C：安全拼接字符串
来源：http://waw.jyoumei.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yvj.bjfxy.top

[S18] C：命令行参数
来源：http://gnw.gogol.net.cn

int main(int argc, char **argv)
来源：http://ikf.hammf.cn

[S19] C：快速排序
来源：http://rqb.jianghu66.top

qsort(a, n, sizeof(int), cmp);
来源：http://ptj.316326.xyz

[S20] C：二分查找
来源：http://uhf.wangshuangyany.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://itg.zhiwuduotai.top

[S21] C：字符类别判断
来源：http://pgy.ybcxt.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://icn.aizwys.cn

[S22] C：字符串转数字
来源：http://lrn.ctjpmb.com

atoi("42");  strtod("3.14", NULL);
来源：http://ccx.hfpthk.cn

[S23] C：随机数
来源：http://fli.xinyue.icu

srand(time(NULL));  int r = rand() % 100;
来源：http://kyx.fengsongda.top

[S24] C：获取本地时间
来源：http://jpy.zhiwuduotai.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mjw.cucudq.cn

[S25] C：内存拷贝
来源：http://dna.daxiang520.top

memcpy(dst, src, n);
来源：http://rxm.jiagoushi.top

[S26] C：内存清零
来源：http://scf.xziqi.cn

memset(a, 0, sizeof a);
来源：http://pee.wangdashe.top

[S27] C：定义常量
来源：http://jhw.aizwys.cn

const double PI = 3.14159;
来源：http://aly.haohaochexian.top

[S28] C：静态变量
来源：http://nsp.ybcxt.top

static int counter = 0;
来源：http://tvy.zdbjq.cn

[S29] C：变参函数
来源：http://swh.pengpengdd.cyou

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bor.zhijiandao.cn

[S30] C：头文件保护
来源：http://yuf.0kj1m.cn

#ifndef X_H
来源：http://dnj.zdbjq.cn

#define X_H
来源：http://xvx.daxiang520.top

#endif
来源：http://eqw.xylfe.cn

[S31] C++：Hello World
来源：http://jtz.nanxuanxn.top


<!-- 参考信息 -->
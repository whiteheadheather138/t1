代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lef.tarul.cn

[Q56] 密集排名（并列不占位）
来源：http://wye.ehwqpu.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wog.zdqjudy.top

[Q57] 行号
来源：http://epd.gogol.net.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kts.yueranfly.top

[Q58] 累计求和
来源：http://rtz.zhaomingkeji.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zim.zycfv.cn

[Q59] 分组内累计
来源：http://ywu.wangshuangyany.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pfy.cashguo.top

[Q60] 取上一行 / 下一行
来源：http://fvw.hcnkem.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xdd.ydjk.org.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bkt.sweek.top

[Q61] 移动平均
来源：http://kmt.c1oappe.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pue.ehwqpu.com

[Q62] 分组占比
来源：http://gfs.gogol.net.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nli.shangyingyoupin.top

[Q63] 开启事务
来源：http://hho.daxiang520.top

START TRANSACTION;                -- 或 BEGIN
来源：http://gap.feifeiyinyue.top

[Q64] 提交事务
来源：http://jdu.tian-w.cn

COMMIT;
来源：http://gxw.jianghu66.top

[Q65] 回滚事务
来源：http://nbl.nanxuanxn.top

ROLLBACK;
来源：http://uik.pengpengdd.cyou

[Q66] 行锁查询
来源：http://tbr.zhongyouzk.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dvt.cucudq.cn

[Q67] 设置隔离级别
来源：http://mrd.vehdjk.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://par.yuanzhike.top

[Q68] 保存点
来源：http://sfj.xylfe.cn

SAVEPOINT sp1;
来源：http://too.quarkkingdee.top

ROLLBACK TO sp1;
来源：http://seb.yj202588.top

[Q69] 查看执行计划
来源：http://sco.ydjk.org.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gfp.316326.xyz

[Q70] 更新统计信息
来源：http://zer.hcnkem.com

ANALYZE TABLE users;
来源：http://cdt.haohaochexian.top

[Q71] 查看建表语句
来源：http://wnz.uphjek.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vcw.zdbjq.cn

[Q72] 查看索引
来源：http://ryd.hcnkem.com

SHOW INDEX FROM users;
来源：http://bvo.andypj.xyz

[Q73] 查看表状态
来源：http://zrs.ybcxt.top

SHOW TABLE STATUS LIKE 'users';
来源：http://tzq.chenjidiqi.icu

[Q74] 强制使用索引
来源：http://hme.hesvh.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tpp.birdmap.top

[Q75] 日期格式化
来源：http://cye.52xcode.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ksw.quarkkingdee.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tss.hnxiangtu.top

[Q76] 按天统计
来源：http://uqt.feifeiyinyue.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ocg.hcnkem.com

[Q77] 时间加减
来源：http://iuv.quarkkingdee.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gdj.vqdsnc.cn

[Q78] 当前时间
来源：http://wco.shuidangran.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zzt.shangyingyoupin.top

[Q79] 字符串拼接
来源：http://wnx.ppjwa.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xnu.fehbvm.com

[Q80] 字符串截取
来源：http://eln.vehdjk.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kzs.jinghuilouyu.cn

[Q81] 字符串替换
来源：http://qju.52xcode.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vut.jinyuanbaomall.cn

[Q82] 字符长度与字节长度
来源：http://ukq.jyoumei.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mee.shangyingyoupin.top

[Q83] 大小写转换
来源：http://usu.daxiang520.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wso.jinqigfzy.top

[Q84] 去除首尾空格
来源：http://pay.0kj1m.cn

SELECT TRIM(name) FROM users;
来源：http://xfr.smart0.xyz

[Q85] 数值取整
来源：http://bcd.zdqjudy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://twr.guannengcc.top

[Q86] 读取 JSON 字段
来源：http://wfk.xinyue.icu

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wzx.haohaochexian.top

[Q87] JSON 字段做条件
来源：http://udo.jinghuilouyu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://emj.jyoumei.cn

[Q88] 行转列（条件聚合）
来源：http://vxh.sjlbkw.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qnr.bjfxy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hqm.shangyingyoupin.top

[Q89] 判断表是否存在
来源：http://dtp.vqdsnc.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nrj.vehdjk.com

[Q90] 生成序号列
来源：http://szr.yongpay.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ivb.cucudq.cn

================================================================================
来源：http://xym.fzhhl.top

R. Bash 专题
来源：http://baa.wangshuangyany.cn

================================================================================
来源：http://jbq.ivvv.top

[R01] shebang 与严格模式
来源：http://cgc.sxryk.cn

#!/usr/bin/env bash
来源：http://aml.cqqwz.cn

set -euo pipefail
来源：http://moq.chenjidiqi.icu

[R02] 变量赋值与使用
来源：http://cwc.guowangkeji.top

name="Tom"; echo "$name"
来源：http://xpu.dianchejie.cn

[R03] 只读变量
来源：http://amz.haohaochexian.top

readonly PI=3.14
来源：http://owo.fanxiaobao.xyz

[R04] 位置参数
来源：http://fwx.xuetiantiany.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rgx.guowangkeji.top

[R05] 参数默认值
来源：http://qnm.sweek.top

name="${1:-default}"
来源：http://cqr.jinyuanbaomall.cn

[R06] 判断命令是否存在
来源：http://tpl.yfazqb.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fup.tian-w.cn

[R07] if 判断文件
来源：http://sud.hfpthk.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://act.ydjk.org.cn

[R08] 数值比较
来源：http://zbv.aizwys.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://wfh.guowangkeji.top

[R09] 字符串比较
来源：http://uww.yj20258.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xrl.pycfn.com

[R10] 正则匹配
来源：http://mpj.quarkkingdee.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://isw.sweek.top

[R11] case 多分支
来源：http://jir.epnwcf.com

case "$1" in
来源：http://lmj.jianghu66.top

start) echo "启动" ;;
来源：http://fee.ehwqpu.com

stop)  echo "停止" ;;
来源：http://jki.xziqi.cn

*)     echo "未知命令" ;;
来源：http://puf.chenlongwang.top

esac
来源：http://amg.sysykeji.top

[R12] for 遍历文件
来源：http://znp.cashguo.top

for f in *.txt; do echo "$f"; done
来源：http://eoy.iojbl.cn

[R13] for 计数循环
来源：http://gyo.guowangkeji.top

for i in {1..10}; do echo "$i"; done
来源：http://jey.jqgfzy.top

[R14] C 风格 for
来源：http://vfi.zycfv.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sxs.bjfxy.top

[R15] while 逐行读文件
来源：http://eaw.dianchejie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yxp.xziqi.cn

[R16] until 等待条件
来源：http://yjo.yuxming.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wgg.cucudq.cn

[R17] 数组定义与取值
来源：http://llz.dianchejie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://pbb.guannengcc.top

[R18] 遍历数组
来源：http://lsi.yj20258.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jrw.yongpay.top

[R19] 数组长度
来源：http://ebm.yj20258888.top

echo "${#arr[@]}"
来源：http://bum.ywan-chungtsiang.top

[R20] 关联数组（字典）
来源：http://egl.yuanzhike.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ing.guowangkeji.top

[R21] 字符串长度
来源：http://cfc.fengsongda.top

echo "${#s}"
来源：http://kct.havefunace.top

[R22] 截取子串
来源：http://dqq.fzhhl.top

echo "${s:0:5}"
来源：http://hdn.jlsjyb.cn

[R23] 字符串替换
来源：http://ziz.gogol.net.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rcp.zhijiandao.cn

[R24] 大小写转换
来源：http://nsm.jinqigufen.top

echo "${s^^}"; echo "${s,,}"
来源：http://yvo.chenjidiqi.icu

[R25] 去后缀 / 去前缀
来源：http://krn.guannengcc.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://byz.aizwys.cn

[R26] 命令替换
来源：http://xht.mhx1999.top

now=$(date +%F); echo "$now"
来源：http://cuc.daxiang520.top

[R27] 算术展开
来源：http://uud.fengsongda.top

echo $((1 + 2 * 3))
来源：http://wfk.shanyushiyangkeji.top

[R28] 浮点运算
来源：http://xwo.zdbjq.cn

echo "scale=2; 10/3" | bc
来源：http://kov.ivvv.top

[R29] 定义函数
来源：http://jxt.fanxiaobao.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bzj.jinqigufen.top

[R30] 函数返回状态码
来源：http://byk.zhixingplan.top

f() { return 0; }; f || echo "失败了"
来源：http://xsy.gaohongyu789.top

[R31] 局部变量
来源：http://lsf.nanxuanxn.top

f() { local x=1; echo "$x"; }
来源：http://zfm.yueranfly.top

[R32] 参数个数校验
来源：http://mty.gaohongyu789.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mse.guannengcc.top

[R33] 捕获错误并提示行号
来源：http://mfm.yj20258.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qar.birdmap.top

[R34] 退出时清理
来源：http://srz.svipenyu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://chg.shanyushiyangkeji.top

[R35] 后台执行并等待
来源：http://eoo.cashguo.top

sleep 5 & pid=$!; wait "$pid"
来源：http://plf.yfazqb.com

[R36] 并发执行多个任务
来源：http://jdq.fktsv.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fgb.chenzaomai.com

[R37] 把输出赋给变量
来源：http://fdj.jinyuanbaomall.cn

files=$(ls -1)
来源：http://gkr.cqqwz.cn

[R38] 管道串联
来源：http://zhx.tian-w.cn

cat a.txt | grep -i error | wc -l
来源：http://ypt.cashguo.top

[R39] 重定向标准输出与错误
来源：http://wsh.cashguo.top

cmd > out.log 2>&1
来源：http://yal.havefunace.top

[R40] 追加写日志
来源：http://nvs.dashuyun.cn

echo "log" >> out.log
来源：http://ppi.svipenyu.cn

[R41] 丢弃输出
来源：http://lne.uphjek.com

cmd >/dev/null 2>&1
来源：http://ykh.vqdsnc.cn

[R42] 输入重定向
来源：http://ehj.gotoacloud.top

wc -l < a.txt
来源：http://uep.xingfuxueyuan.xyz

[R43] 按名字查找文件
来源：http://kad.ydjk.org.cn

find . -name "*.log" -type f
来源：http://cnb.haohaochexian.top

[R44] 按修改时间查找
来源：http://kxz.xingfuxueyuan.xyz

find . -mtime -7 -type f
来源：http://udl.cucudq.cn

[R45] 批量删除
来源：http://tmq.c1oappe.top

find . -name "*.tmp" -delete
来源：http://wpe.smart0.xyz

[R46] 递归替换文件内容
来源：http://fro.jlsjyb.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fea.quarkkingdee.top

[R47] sed 单行替换
来源：http://sdk.gaohongyu789.top

sed -i 's/foo/bar/g' a.txt
来源：http://fkt.sufxvd.cn

[R48] awk 取指定列
来源：http://ouw.shangyingyoupin.top

awk '{print $1, $3}' a.txt
来源：http://mmn.gzhubu.top

[R49] awk 带条件
来源：http://okj.nanxinkj.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rjk.yongpay.top

[R50] awk 求和
来源：http://yvx.zhaomingkeji.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://qqy.ywan-chungtsiang.top

[R51] 排序去重取前几
来源：http://otj.hysaishi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ywc.shanyushiyangtech.top

[R52] 统计行数
来源：http://tbi.guowangkeji.top

wc -l a.txt
来源：http://vgx.bjfxy.top

[R53] 查看文件头与实时尾
来源：http://xfn.yanxiufei.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ibw.sweek.top

[R54] 比较两个文件
来源：http://rtn.feifeiyinyue.top

diff a.txt b.txt
来源：http://ado.tian-w.cn

[R55] 压缩与解压
来源：http://sxt.yfazqb.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jzu.cqqwz.cn

[R56] 远程拷贝
来源：http://ypx.zhijiandao.cn

scp file user@host:/path/
来源：http://tqf.sufxvd.cn

[R57] 远程执行命令
来源：http://mvw.zhiwuduotai.top

ssh user@host 'uptime'
来源：http://cbf.uphjek.com

[R58] 下载文件
来源：http://kii.ywan-chungtsiang.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nuw.nwbrower.top

[R59] 发 POST JSON
来源：http://sfg.xingfuxueyuan.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jlj.nanxuanxn.top

[R60] 只看 HTTP 状态码
来源：http://xck.birdmap.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hmo.ydjk.org.cn

[R61] 磁盘占用
来源：http://fww.redwolf501.top

df -h;  du -sh *
来源：http://uwc.gaohongyu789.top

[R62] 找最占空间的文件
来源：http://uvg.gaohongyu789.top

du -ah . | sort -rh | head -10
来源：http://ptk.yongpay.top

[R63] 内存与进程
来源：http://tky.wangdashe.top

free -h;  ps aux | grep nginx
来源：http://qsc.yvedp.cn

[R64] 结束进程
来源：http://pmv.quarkkingdee.top

kill -9 $(pgrep -f app.py)
来源：http://obs.gotoacloud.top

[R65] 查看端口占用
来源：http://brh.yj202588.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ygh.shanyushiyangkeji.top

[R66] 定时任务
来源：http://sxr.yj20258.top

crontab -e;  crontab -l
来源：http://omz.chenzaomai.com

[R67] 生成随机十六进制串
来源：http://kxd.yuanzhike.top

openssl rand -hex 16
来源：http://qvj.ivvv.top

[R68] 计算文件校验值
来源：http://tiw.pengpengdd.cyou

sha256sum a.txt;  md5sum a.txt
来源：http://sdu.epnwcf.com

[R69] 生成随机密码
来源：http://ygz.cdnleiting.top

head -c 16 /dev/urandom | base64
来源：http://lkd.nanxuanxn.top

[R70] 时间戳与互转
来源：http://pkd.gotoacloud.top

date +%s;  date -d @1700000000
来源：http://isx.jinyuanbaomall.cn

[R71] 日期格式化
来源：http://giu.cashguo.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://qfb.hnxiangtu.top

[R72] 等待端口就绪
来源：http://rbf.uphjek.com

until nc -z localhost 3306; do sleep 1; done
来源：http://tyw.zhongyouzk.top

[R73] 分割大日志
来源：http://agy.c1oappe.top

split -l 1000 big.log part_
来源：http://ddi.cashguo.top

[R74] 批量重命名
来源：http://wxu.jinyuanbaomall.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ruf.chenzaomai.com

[R75] 导出环境变量
来源：http://ccm.fktsv.cn

export PATH="$HOME/bin:$PATH"
来源：http://dgh.hcnkem.com

[R76] 使用临时文件
来源：http://lxz.hongshengwenyu.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ddw.shangyingyoupin.top

[R77] 读取用户输入
来源：http://mmc.wangshuangyany.cn

read -rp "请输入: " ans
来源：http://xwt.svipenyu.cn

[R78] 交互式菜单
来源：http://mii.zhiwuduotai.top

select opt in a b c; do echo "$opt"; break; done
来源：http://vrw.yj20258888.top

[R79] 解析命令行选项
来源：http://vmq.svipenyu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ixx.gotoacloud.top

[R80] 查看脚本执行耗时
来源：http://vdt.chenzaomai.com

time ./run.sh
来源：http://nce.zhixingplan.top

================================================================================
来源：http://bgx.jinyuanbaomall.cn

S. C / C++ 专题
来源：http://hpi.xinyue.icu

================================================================================
来源：http://mlr.cheryme.top

[S01] C：Hello World
来源：http://hjy.xingfuxueyuan.xyz

#include <stdio.h>
来源：http://duz.bjfxy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://nno.cqqwz.cn

[S02] C：变量与格式化输出
来源：http://tzl.sjlbkw.cn

int a = 10; printf("%d\n", a);
来源：http://zme.cashguo.top

[S03] C：读入整数
来源：http://amt.hnxiangtu.top

int x; scanf("%d", &x);
来源：http://hpg.birdmap.top

[S04] C：字符串复制
来源：http://bes.yj202588.top

char dst[32]; strcpy(dst, "hi");
来源：http://deg.havefunace.top

[S05] C：字符串长度
来源：http://fzo.yanxiufei.cn

strlen(s)
来源：http://grv.xinyue.icu

[S06] C：字符串比较
来源：http://bhq.jinqigfzy.top

strcmp(a, b) == 0
来源：http://jbw.iojbl.cn

[S07] C：数组遍历求和
来源：http://teh.gotoacloud.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://obu.jqgufenzy.top

[S08] C：动态内存分配与释放
来源：http://aod.shanyushiyangkeji.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dbp.yonumen.top

[S09] C：结构体定义与初始化
来源：http://qtd.tarul.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dab.gzhubu.top

[S10] C：指针与解引用
来源：http://lcl.fehbvm.com

int *p = &a;  *p = 5;
来源：http://dja.yfazqb.com

[S11] C：逐行读文件
来源：http://qoo.ydjk.org.cn

FILE *f = fopen("a.txt", "r");
来源：http://qmy.yueranfly.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://vpr.cdnleiting.top

fclose(f);
来源：http://bpt.redwolf501.top

[S12] C：写文件
来源：http://rso.redwolf501.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gyq.jqgfzy.top

[S13] C：宏定义
来源：http://msg.kuanghao11.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dfh.xylfe.cn

[S14] C：枚举
来源：http://qzn.jiagoushi.top

enum Color { RED, GREEN, BLUE };
来源：http://huc.yj202588.top

[S15] C：类型转换
来源：http://saa.hywenlv.cn

(double) a / b
来源：http://yio.bbcook.cn

[S16] C：位操作置位
来源：http://ojm.meibo888.top

x |= (1 << 3);
来源：http://fci.xuetiantiany.cn

[S17] C：安全拼接字符串
来源：http://mkf.ppjwa.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xqb.chenzaomai.com

[S18] C：命令行参数
来源：http://byt.xylfe.cn

int main(int argc, char **argv)
来源：http://uoh.hnqzz.top

[S19] C：快速排序
来源：http://kvc.jqgufenzy.top

qsort(a, n, sizeof(int), cmp);
来源：http://vnf.ydjk.org.cn

[S20] C：二分查找
来源：http://oxo.xuetiantiany.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lyx.zhongyouzk.top

[S21] C：字符类别判断
来源：http://tgt.bbcook.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mav.jinyuanbaomall.cn

[S22] C：字符串转数字
来源：http://tck.daxiang520.top

atoi("42");  strtod("3.14", NULL);
来源：http://dyz.tian-w.cn

[S23] C：随机数
来源：http://ycq.daxiang520.top

srand(time(NULL));  int r = rand() % 100;
来源：http://eai.zhaomingkeji.xyz

[S24] C：获取本地时间
来源：http://qau.gogol.net.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mxd.guowangkeji.top

[S25] C：内存拷贝
来源：http://hal.gzhubu.top

memcpy(dst, src, n);
来源：http://umb.xuetiantiany.cn

[S26] C：内存清零
来源：http://vde.fehbvm.com


<!-- 参考信息 -->